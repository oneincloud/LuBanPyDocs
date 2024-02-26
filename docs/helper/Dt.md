# Dt - 日期时间组件

## TODO清单：

- [ ] tzinfo - 获取时区对象
- [ ] localzone - 获取当前系统时区
- [ ] now - 获取当前系统时间
- [ ] today - 获取当前日期
- [ ] strtotime - 将字符串解释为Unix时间戳
- [ ] parse - 解释为datetime对象
- [ ] format - 将日期格式化为自符串



## toTimezone - 转换为timezone对象

将ZoneId、UTC偏移量、国家代码等转换为`timezone`对象。

| 偏移量表示法 | 描述                                     |
| ------------ | ---------------------------------------- |
| GMT+8        | 相对GMT多8个小时                         |
| Etc/GMT-8    | 同GMT+8，+-号相反                        |
| UTC+8        | 同GMT+8                                  |
| GMT+08:00    | 精确到分钟级别                           |
| GMT+08:00:00 | 精确到秒级别                             |
| GMT+0800     | 精确到分钟级别，省略冒号                 |
| GMT+080000   | 精确到秒级别，省略冒号                   |
| +08:00       | 精确到分钟级别，省略前缀                 |
| +08:00:00    | 精确到秒级别，省略前缀                   |
| +0800        | 精确到分钟级别，省略前缀与冒号           |
| +080000      | 精确到秒级别，省略前缀与冒号             |
| Z            | 表示零时区，等同于GMT、UTC、GMT+0、UTC+0 |



```python
def toTimezone(tz) -> Optional[datetime.tzinfo]:
```

### - 参数说明

| 参数 | 类型                        | 必选 | 默认值 | 说明     |
| ---- | --------------------------- | ---- | ------ | -------- |
| tz   | [int, str, datetime.tzinfo] | Y    |        | 时间信息 |

### - 使用示例





## getTimeZone - 获取当前系统时区





## setTimeZone - 设置当前系统时区





## parse - 解释为datetime对象

`parse`方法尝试将不同的类型统一解释为`datetime`对象返回，无法解释时返回`None`

```python
def parse(cls, val, fmt: Optional[str] = None, tz: Union[str, int, datetime.tzinfo] = None) -> Optional[datetime.datetime]
```

### - 参数说明

| 参数 | 类型                                                         | 必选 | 默认值 | 说明               |
| ---- | ------------------------------------------------------------ | ---- | ------ | ------------------ |
| val  | [str, int, float, datetime.datetime, datetime.date, time.struct_time] | Y    | 无     | 需要解释的对象     |
| fmt  | str                                                          | N    | 无     | 指字符串的时间格式 |

### - 使用示例

##### 示例一、内置时间类型相互转换

```python
# 时间戳
Date.parse(1662799891)				# 结果：2022-09-10 16:51:31
Date.parse(1662799891.123)			# 结果：2022-09-10 16:51:31.123000

# datetime
Date.parse(Date.now())				# 结果：2022-09-10 20:33:47.209026

# date
dt4 = Date.parse(Date.today())		# 结果：2022-09-10 00:00:00

# struct_time
Date.parse(time.localtime())		# 结果：2022-09-10 20:33:47
```

##### 示例二：使用dateutil模块解释

parser是根据字符串解析成datetime,字符串可以很随意，可以用时间日期的英文单词，可以用横线、逗号、空格等做分隔符。
没指定时间默认是0点，没指定日期默认是今天，没指定年份默认是今年。

```python
Date.parse("2018-10-21")			# 结果：2018-10-21 00:00:00
Date.pares("20181021")				# 结果：2018-10-21 00:00:00
Date.parse('2018/10/21')			# 结果：2018-10-21 00:00:00
Date.parse('10-21')					# 结果：2022-10-21 00:00:00

Date.parse('2022-9-10 21:12:12')	# 结果：2022-09-10 21:12:12
Date.parse('2022-9-10 21:12')		# 结果：2022-09-10 21:12:00
Date.parse('2022-9-10 21')			# 结果：2022-09-10 21:00:00
```

##### 示例三：使用dateparser模块解释

> https://github.com/scrapinghub/dateparser

```python
Date.parse("1 min ago")
Date.parse("2 weeks ago")
Date.parse("3 months, 1 week and 1 day ago")
Date.parse("in 2 days")
Date.parse("tomorrow")
Date.parse("21 July 2013 10:15 pm +0500")
```

##### 示例四：周期起始日期、结束日期

需要`first of` 或 `end of` 开头

* 翻译参数

  ```python
  _trans = {
  	'period': {      # 周期
      	'week': ['周', 'weeks'],
          'month': ['月', 'months'],
          'season': ['季', '季度', 'seasons', 'quarter', 'quarter'],
          'year': ['年', 'years']
  	},
      'around': {
      	'this': ['本', '今'],
          'last': ['上', '之前', '前'],
          'next': ['下', '之后', '后']
  	},
      'suffix': {
      	'first': ['开始', '首日', '起', '首', 'start'],
          'end': ['结束', '最后', '未', '尾', 'start']
  	}
  }
  ```

* 不带参考日期时间

  * En文法

    ```python
    # 英文测试
    for _around in ['this', 'last', 'next']:
    	for _period in ['week', 'month', 'season', 'year']:
        	for _suffix in ['first', 'end']:
            	val = f'{_suffix} of {_around} {_period}'
                _dt = Date.parse(val)
                print("'%s' 结果（%s）：" % (val, type(_dt)), _dt)
                
    # 返回结果：
    """
    'first of this week' 结果（<class 'datetime.datetime'>）： 2022-09-12 00:46:28
    'end of this week' 结果（<class 'datetime.datetime'>）： 2022-09-18 00:46:28
    'first of this month' 结果（<class 'datetime.datetime'>）： 2022-09-01 00:46:28
    'end of this month' 结果（<class 'datetime.datetime'>）： 2022-09-30 00:46:28
    'first of this season' 结果（<class 'datetime.datetime'>）： 2022-07-01 00:46:28
    'end of this season' 结果（<class 'datetime.datetime'>）： 2022-09-30 00:46:28
    'first of this year' 结果（<class 'datetime.datetime'>）： 2022-01-01 00:46:28
    'end of this year' 结果（<class 'datetime.datetime'>）： 2022-12-31 00:46:28
    'first of last week' 结果（<class 'datetime.datetime'>）： 2022-09-05 00:46:28
    'end of last week' 结果（<class 'datetime.datetime'>）： 2022-09-11 00:46:28
    'first of last month' 结果（<class 'datetime.datetime'>）： 2022-08-01 00:46:28
    'end of last month' 结果（<class 'datetime.datetime'>）： 2022-08-31 00:46:28
    'first of last season' 结果（<class 'datetime.datetime'>）： 2022-04-01 00:46:28
    'end of last season' 结果（<class 'datetime.datetime'>）： 2022-06-30 00:46:28
    'first of last year' 结果（<class 'datetime.datetime'>）： 2021-01-01 00:46:28
    'end of last year' 结果（<class 'datetime.datetime'>）： 2021-12-31 00:46:28
    'first of next week' 结果（<class 'datetime.datetime'>）： 2022-09-19 00:46:28
    'end of next week' 结果（<class 'datetime.datetime'>）： 2022-09-25 00:46:28
    'first of next month' 结果（<class 'datetime.datetime'>）： 2022-10-01 00:46:28
    'end of next month' 结果（<class 'datetime.datetime'>）： 2022-10-31 00:46:28
    'first of next season' 结果（<class 'datetime.datetime'>）： 2022-10-01 00:46:28
    'end of next season' 结果（<class 'datetime.datetime'>）： 2022-12-31 00:46:28
    'first of next year' 结果（<class 'datetime.datetime'>）： 2023-01-01 00:46:28
    'end of next year' 结果（<class 'datetime.datetime'>）： 2023-12-31 00:46:28
    """
    ```

  * 中文文法

    ```python
    for _around in ['本', '上', '下']:
    	for _period in ['周', '月', '季', '年']:
        	for _suffix in ['开始', '结束']:
            	val = f'{_around}{_period}{_suffix}'
                _dt = Date.parse(val)
                print("'%s' 结果（%s）：" % (val, type(_dt)), _dt)
                
    # 返回结果：
    """
    '本周开始' 结果（<class 'datetime.datetime'>）： 2022-09-12 00:56:04
    '本周结束' 结果（<class 'datetime.datetime'>）： 2022-09-18 00:56:04
    '本月开始' 结果（<class 'datetime.datetime'>）： 2022-09-01 00:56:04
    '本月结束' 结果（<class 'datetime.datetime'>）： 2022-09-30 00:56:04
    '本季开始' 结果（<class 'datetime.datetime'>）： 2022-07-01 00:56:04
    '本季结束' 结果（<class 'datetime.datetime'>）： 2022-09-30 00:56:04
    '本年开始' 结果（<class 'datetime.datetime'>）： 2022-01-01 00:56:04
    '本年结束' 结果（<class 'datetime.datetime'>）： 2022-12-31 00:56:04
    '上周开始' 结果（<class 'datetime.datetime'>）： 2022-09-05 00:56:04
    '上周结束' 结果（<class 'datetime.datetime'>）： 2022-09-11 00:56:04
    '上月开始' 结果（<class 'datetime.datetime'>）： 2022-08-01 00:56:04
    '上月结束' 结果（<class 'datetime.datetime'>）： 2022-08-31 00:56:04
    '上季开始' 结果（<class 'datetime.datetime'>）： 2022-04-01 00:56:04
    '上季结束' 结果（<class 'datetime.datetime'>）： 2022-06-30 00:56:04
    '上年开始' 结果（<class 'datetime.datetime'>）： 2021-01-01 00:56:04
    '上年结束' 结果（<class 'datetime.datetime'>）： 2021-12-31 00:56:04
    '下周开始' 结果（<class 'datetime.datetime'>）： 2022-09-19 00:56:04
    '下周结束' 结果（<class 'datetime.datetime'>）： 2022-09-25 00:56:04
    '下月开始' 结果（<class 'datetime.datetime'>）： 2022-10-01 00:56:04
    '下月结束' 结果（<class 'datetime.datetime'>）： 2022-10-31 00:56:04
    '下季开始' 结果（<class 'datetime.datetime'>）： 2022-10-01 00:56:04
    '下季结束' 结果（<class 'datetime.datetime'>）： 2022-12-31 00:56:04
    '下年开始' 结果（<class 'datetime.datetime'>）： 2023-01-01 00:56:04
    '下年结束' 结果（<class 'datetime.datetime'>）： 2023-12-31 00:56:04
    """
    ```

* 指定参考日期和时间

  ```python
  _with = [
  	'本周开始 2021-2-28',
      '下月结束 2021-10-1',
      '2年后开始 2021-6-22 10:15'
  ]
  for _t in _with:
  	_dt = Date.parse(_t)
      print("'%s' 结果（%s）：" % (_t, type(_dt)), _dt)
      
  # 返回结果：
  """
  '本周开始 2021-2-28' 结果（<class 'datetime.datetime'>）： 2021-02-22 00:00:00
  '下月结束 2021-10-1' 结果（<class 'datetime.datetime'>）： 2021-11-30 00:00:00
  '2年后开始 2021-6-22 10:15' 结果（<class 'datetime.datetime'>）： 2023-01-01 10:15:00
  """
  ```

* 只指定参考时间

  ```python
  _with = [
  	'上周结束 6:00',
      '本季结束 15:30:55',
  ]
  for _t in _with:
  	_dt = Date.parse(_t)
      print("'%s' 结果（%s）：" % (_t, type(_dt)), _dt)
      
  # 返回结果：
  """
  '上周结束 6:00' 结果（<class 'datetime.datetime'>）： 2022-09-11 06:00:00
  '本季结束 15:30:55' 结果（<class 'datetime.datetime'>）： 2022-09-30 15:30:55
  """
  ```

日期时间段可支持任何的解释格式字符，是嵌套调用parse方法进行提取。



## format - 格式为字符串类型

将datetime类型按指格式为字符串





# 附件A：时区概念

### Python使用到的时间相关函数及概念

* 包含时区信息的datetime称为: offset-aware datetime
* 反之称为offset-naive datetime
* datetime.now(): 生成当前默认时区的 naive datetime
* datetime.now(tzinfo=tz): 生成指定时区的offset-aware datetime
* datetime.replace(tzinfo=tz): 直接替换datetime 时区信息为tz时区offset-aware datetime--不针对时区进行任何转换
* datetime.astimezone(tz): 将时间转换为新的tz时区的offset-aware datetime
* naive和aware的datetime是不可以执行比较、相减相关操作的，只有同类型的datetime才能求时间差值、比较大小



## 统一概念

### 标准时间

- 可以理解为世界时间，不存在时区问题
- UTC：(Universal Time Coordinated)，协调世界时。全世界统一的世界标准时间。需要不规则地加入闰秒。
- GMT：(Greenwich Mean Tim)，格林尼治平均时间。
  - 一般认为UTC和GMT是相等的，但是会存在0.9秒以内的误差，这是由于地球不规则自转引起的。

### 时区

- **本地时间：**，UTC+时区，东为正西为负。比如北京时间在东八区就是 UTC+(+0800)。
- **CST 中国基准时间**：为 UTC 时间 + 8 小时，即 UTC 时间的 0 点对应于中国基准时间的 8 点，即为一般称为东八区的时间
- **DST：，夏令时**。是指夏天太阳升起比较早，将时钟拨快一个小时来提早日光的使用。欧美主要国家都引用了这个做法。如果在夏令时时区内 DST=UTC+时区+1。

### 时间戳

1970年1月1日 00:00:00 UTC+00:00时区的时刻称为epoch time，记为0，当前的时间戳即为从 epoch time 到现在的秒数，一般叫做 timestamp，因此一个时间戳一定对应于一个特定的 UTC 时间，同时也对应于其他时区的一个确定的时间。因此时间戳可以认为是一个相对安全的时间表示方法。

- 由UTC世界标准时间转换而来，不带时区；同一时刻获取的时间戳在全世界都是相同的。
- **Unix时间戳：** 表示从UTC1970年1月1日0时0分0秒起至现在的总秒数，不考虑闰秒
- **时间戳：** 表示从UTC1970年1月1日0时0分0秒起至现在的毫秒数。



### 字符串表示

为了让时间易于阅读又出现了用各种字符串来表示时间的方法。

#### RFC2822

> 官方白皮书：https://tools.ietf.org/html/rfc2822#page-14

```js
YYYY/MM/DD HH:MM:SS ± timezone(时区用4位数字表示)
//  1992/02/12 12:23:22+0800
```

#### ISO 8601

> 维基百科：https://zh.wikipedia.org/wiki/ISO_8601

```js
YYYY-MM-DDThh:mm:ss ± timezone(时区用HH:MM表示)

1997-07-16T08:20:30Z
// “Z”表示UTC标准时区，即"00:00",所以这里表示零时区的`1997年7月16日08时20分30秒`
// 日期时间合并表示时，要在时间前面加一大写字母T

// 如要表示东八区时间2004年5月3日下午5点30分8秒，可以写成
2004-05-03T17:30:08+08:00
20040503T173008+08
```



### CST 中国基准时间

为 UTC 时间 + 8 小时，即 UTC 时间的 0 点对应于中国基准时间的 8 点，即为一般称为东八区的时间

### ISO 8601

一种标准化的时间表示方法，表示格式为 ：YYYY-MM-DDThh:mm:ss ± timezone，可以表示不同时区的时间，时区部分用Z 表示为 UTC 标准时区。两个例子：

- 1997-07-16T08:20:30Z 表示的是 UTC 时间的 1997 年 7 月 16 号 8:20:30
- 1997-07-16T19:20:30+08:00 表示的是东八区时间的 1997 年 7 月 16 号 19:20:30



# 参考

* [2w字长文详细介绍 Python 处理日期与时间，这篇太给力了！](https://zhuanlan.zhihu.com/p/412552917)
* [怎么在python中对时区进行设置](https://www.yisu.com/zixun/372628.html)
* [我是如何完美解决Python运行的时区问题的？](https://zhuanlan.zhihu.com/p/415539242)
* [python时区运算，时区，时间戳，夏令时讲解](https://blog.csdn.net/weixin_39925696/article/details/105585572)
* [ISO 3166 国家地区码](https://www.jianshu.com/p/9911b2b4d857)
* [Python3中datetime不同时区转换介绍与踩坑](https://www.cnblogs.com/AcAc-t/p/python3_datetime_timezone.html)
* [简述时区问题复杂性来源（Python 版）](https://zhuanlan.zhihu.com/p/355772985)