# Str - 字符串

## TODO功能清单：

- [ ] ascii - 尝试将字符串转换为 ASCII 值
- [x] after - 返回字符串中指定值之后的所有内容
- [x] afterLast - 返回字符串中指定值最后一次出现后的所有内容
- [ ] transliterate
- [x] before - 返回字符串中指定值之前的所有内容
- [x] beforeLast - 返回字符串中指定值最后一次出现前的所有内容
- [x] between - 返回字符串在指定两个值之间的内容
- [x] betweenFirst - 返回字符串在指定两个值之间的最小可能的部分
- [ ] charAt
- [x] find - 获取子字符串在字符串的首次出现位置
- [x] rfind - 获取子字符串在字符串的最后出现位置
- [x] contains - 判断指定字符串中是否包含另一指定字符串
- [ ] ~~containsAll - 用于判断指定字符串是否包含指定数组中的所有值~~
- [ ] ~~convertCase~~
- [ ] excerpt - 提取字符串中给定短语匹配到的第一个片段
- [x] wrap - 用给定字符串包裹字符串
- [ ] ~~is - 用来判断字符串是否与指定模式匹配~~
- [ ] isAscii - 用于判断字符串是否是 7 位 ASCII
- [x] isJson - 确定给定的字符串是否是有效的 JSON
- [ ] isUrl
- [x] length - 获取字符个数
- [x] size - 获取字符串的字节个数
- [x] limit - 将字符串以指定长度进行截断
- [ ] words - 限制字符串中的单词数
- [ ] markdown
- [ ] inlineMarkdown
- [x] mask - 使用重复的字符掩盖字符串的一部分
- [x] match - 返回字符串中和指定正则表达式匹配的部分
- [x] matchAll - 返回包含了字符串中与指定正则表达式匹配部分的集合
- [x] isMatch - 用于判断给定的字符串是否与正则表达式匹配
- [x] padBoth - 在指定字符串的两侧填充上另一字符串
- [x] padLeft - 在指定字符串的左侧填充上另一字符串
- [x] padRight - 在指定字符串的右侧填充上另一字符串
- [ ] parseCallback
- [x] plural - 将单数形式的字符串转换为复数形式
- [ ] pluralStudly - 将以驼峰格式的单数字符串转化为其复数形式
- [x] singular - 将字符串转换为其单数形式
- [x] password - 生成给定长度的安全随机密码
- [x] position - 查找字符串在另一字符串中第一次出现的位置
- [x] positionLast - 查找字符串在另一字符串中最后一次出现的位置
- [x] random - 生成指定长度的随机字符串
- [ ] toStringOr
- [x] replace - 用于替换字符串中的给定字符串
- [x] replaceIgnoreCase - 用于替换字符串中的给定字符串（不区分大小写）
- [x] replaceArray - 使用数组有序的替换字符串中的特定字符
- [x] replaceFirst - 替换字符串中给定值的第一个匹配项
- [x] replaceLast - 替换字符串中最后一次出现的给定值
- [x] replaceStart - 替换字符串开头第一个出现的给定值
- [x] replaceEnd - 如果给定值出现在字符串末尾，则替换最后出现的值
- [x] replaceMatches - 用给定的替换字符串替换与模式匹配的字符串的所有部分
- [x] substrReplace - 替换字符串一部分中的文本
- [x] swap - 替换给定字符串中的多个值
- [ ] repeat
- [ ] prepend - 用于在指定字符串的开头插入另一指定字符串
- [ ] append - 将给定的值附加到字符串
- [x] remove - 用于从字符串中删除给定的值或值数组
- [x] reverse - 反转给定的字符串
- [x] startsWith - 确定给定字符串是否以给定值开头
- [x] endsWith - 用于判断指定字符串是否以另一指定字符串结尾
- [x] start - 给定值的单个实例添加到字符串中
- [x] finish - 将指定的字符串修改为以指定的值结尾的形式
- [x] lower - 用于将字符串转换为小写
- [x] upper - 将给定字符串转换为大写
- [x] headline - 将由大小写、连字符或下划线分隔的字符串转换为空格分隔的字符串，每个单词的首字母大写
- [x] title - 将给定的字符串转换为 `Title Case`
- [ ] slug - 从给定字符串生成 URL 友好的 `“slug”`
- [x] camel - 将指定字符串转换为`camelCase 驼峰式` 表示方法
- [x] snake - 法将给定字符串转换为 `snake_case`
- [x] studly - 将给定字符串转换为 `StudlyCase`
- [x] kebab - 将字符串转换为烤串式（ `kebab-case` ）表示方法
- [x] squish - 删除字符串中所有无关紧要的空白，包括字符串之间的空白
- [x] ucfirst - 返回第一个字符大写的给定字符串
- [x] lcfirst - 返回给定的字符串的第一个字符为小写字母
- [x] substrCount - 返回给定字符串中给定值的出现次数
- [ ] take
- [x] ucsplit - 将给定的字符串按大写字符拆分为数组
- [ ] wordCount - 返回字符串包含的单词数
- [ ] ~~wordWrap~~
- [x] uuid - 生成一个 UUID（版本 4）
- [ ] orderedUuid - 用于生成一个「时间戳优先」的 UUID 
- [x] isUuid - 确定给定的字符串是否是一个 UUID
- [ ] ulid - 生成一个 ULID
- [ ] isUlid - 确定给定的字符串是否一个 ULID
- [x] isEmpty - 确定给定的字符串是否为空
- [x] isNotEmpty - 确定给定的字符串是否不为空
- [ ] flushCache



## ascii - 尝试将字符串转换为 ASCII 值




## after - 返回字符串中指定值之后的所有内容
`after` 方法返回字符串中指定值之后的所有内容。如果字符串中不存在这个值，它将返回整个字符串

```python
def after(subject: str, search: str) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明             |
| ------- | ---- | ---- | ------ | ---------------- |
| subject | str  | Y    |        | 字符串           |
| search  | str  | Y    |        | 指定检索的字符串 |

### - 使用示例

```python
Str.after('This is my name', 'This is')							# ' my name'
Str.after('This is my name', 'That is')							# 'This is my name'
Str.after('AAAAThis is my name', 'This is')						# ' my name'
Str.after('This is my name1 This is my name2', 'This is')		# ' my name1 This is my name2'
```



## afterLast - 返回字符串中指定值最后一次出现后的所有内容

`afterLast` 方法返回字符串中指定值最后一次出现后的所有内容。如果字符串中不存在这个值，它将返回整个字符串

```python
def afterLast(cls, subject: str, search: str) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明             |
| ------- | ---- | ---- | ------ | ---------------- |
| subject | str  | Y    |        | 字符串           |
| search  | str  | Y    |        | 指定检索的字符串 |

### - 使用示例

```python
Str.afterLast(r'App\Http\Controllers\Controller', '\\')		# 'Controller'
```




## transliterate


## before - 返回字符串中指定值之前的所有内容

```python
def before(cls, subject: str, search: str) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明             |
| ------- | ---- | ---- | ------ | ---------------- |
| subject | str  | Y    |        | 字符串           |
| search  | str  | Y    |        | 指定检索的字符串 |

### - 使用示例

```python
Str.before('This is my name', 'my name')		# 'This is '
```



## beforeLast - 返回字符串中指定值最后一次出现前的所有内容

```python
def beforeLast(cls, subject: str, search: str):
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明             |
| ------- | ---- | ---- | ------ | ---------------- |
| subject | str  | Y    |        | 字符串           |
| search  | str  | Y    |        | 指定检索的字符串 |

### - 使用示例

```python
Str.beforeLast('This is my name', 'is')		# 'This '
```



## between - 返回字符串在指定两个值之间的内容

`between` 方法返回两个值之间的字符串部分

```python
def between(cls, subject: str, start: str, end: str):
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明       |
| ------- | ---- | ---- | ------ | ---------- |
| subject | str  | Y    |        | 字符串     |
| start   | str  | Y    |        | 起始字符串 |
| end     | str  | Y    |        | 结束字符串 |

### - 使用示例

```python
Str.between('This is my name', 'This', 'name')		# ' is my '
Str.between('[a] bc [d]', '[', ']')					# 'a] bc [d'
```



## betweenFirst - 返回字符串在指定两个值之间的最小可能的部分

`betweenFirst` 方法返回两个值之间字符串的最小可能部分

```python
def betweenFirst(cls, subject: str, start: str, end: str) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明       |
| ------- | ---- | ---- | ------ | ---------- |
| subject | str  | Y    |        | 字符串     |
| start   | str  | Y    |        | 起始字符串 |
| end     | str  | Y    |        | 结束字符串 |

### - 使用示例

```python
Str.betweenFirst('[a] bc [d]', '[', ']')		# 'a'
```



## charAt


## find - 获取子字符串在字符串的首次出现位置

检测 子字符串是否包含在 字符串 中，如果是返回开始的索引值，否则返回-1

```python
def find(text: str, search: str, caseSensitive: bool = True) -> int:
```

### - 参数说明

| 参数          | 类型 | 必选 | 默认值 | 说明                             |
| ------------- | ---- | ---- | ------ | -------------------------------- |
| text          | str  | Y    |        | 要被检查的 string                |
| search        | str  | Y    |        | 在 text 中查找这个字符串         |
| caseSensitive | bool | N    | True   | 是否大小写母感，默认为区分大小写 |

### - 使用示例

```python
# ASCII测试，区分大小写
Str.find('abcdEFGHijk abcdEFGHijk', 'EF')		# 结果：4

# ASCII测试，不包含
Str.find('abcdEFGHijk abcdEFGHijk', 'ef')		# 结果：-1

# ASCII测试，忽略大小写
Str.find('abcdEFGHijk abcdEFGHijk', 'ef', False)	# 结果：4

# 中文测试
Str.find('你好Python 你好Python', '好P')				# 结果： 1
```



## rfind - 获取子字符串在字符串的最后出现位置

检测 子字符串是否包含在 字符串 中，如果是返回最后的索引值，否则返回-1

```python
def rfind(text: str, search: str, caseSensitive: bool = True) -> int:
```

### - 参数说明

| 参数          | 类型 | 必选 | 默认值 | 说明                             |
| ------------- | ---- | ---- | ------ | -------------------------------- |
| text          | str  | Y    |        | 要被检查的 string                |
| search        | str  | Y    |        | 在 text 中查找这个字符串         |
| caseSensitive | bool | N    | True   | 是否大小写母感，默认为区分大小写 |

### - 使用示例

```python
# ASCII测试，区分大小写
Str.rfind('abcdEFGHijk abcdEFGHijk', 'EF')		# 结果：16

# ASCII测试，不包含
Str.rfind('abcdEFGHijk abcdEFGHijk', 'ef')		# 结果：-1

# ASCII测试，忽略大小写
Str.rfind('abcdEFGHijk abcdEFGHijk', 'ef', False)	# 结果：16

# 中文测试
Str.rfind('你好Python 你好Python', '好P')				# 结果： 10
```



## contains - 判断指定字符串中是否包含另一指定字符串

`contains` 方法判断指定字符串中是否包含另一指定字符串或一组字符串（默认区分大小写），可通过设置第三个参数`ignoreCase`为`True`忽略大小写。

```python
def contains(haystack: str, needles: Union[str, Tuple[str], List[str], Set[str]], ignoreCase: bool = False) -> bool:
```

### - 参数说明

| 参数       | 类型                                        | 必选 | 默认值 | 说明                           |
| ---------- | ------------------------------------------- | ---- | ------ | ------------------------------ |
| haystack   | str                                         | Y    |        | 字符串                         |
| needles    | Union[str, Tuple[str], List[str], Set[str]] | Y    |        | 子字符串或数组                 |
| ignoreCase | bool                                        | N    | False  | 是否区分大小写，默认区分大小写 |

### - 使用示例

```python
Str.contains('This is my name', 'my')				# True
Str.contains('This is my name', ['my', 'foo'])		# True
Str.contains('This is my name', 'My')				# False
Str.contains('This is my name', 'My', True)			# True
```



## convertCase
## excerpt - 提取字符串中给定短语匹配到的第一个片段


## wrap - 用给定字符串包裹字符串

```python
def wrap(value: str, before: str, after: Optional[str] = None) -> str:
```

### - 参数说明

| 参数   | 类型          | 必选 | 默认值 | 说明                             |
| ------ | ------------- | ---- | ------ | -------------------------------- |
| value  | str           | Y    |        | 字符串                           |
| before | str           | Y    |        | 前缀字符串                       |
| after  | Optional[str] | N    | None   | 后缀字符串，未设置时使用`before` |

### - 使用示例

```python
Str.wrap('word', '#')				# '#word#'
Str.wrap('word', '[', ']')			# '[word]'
```



## is - 用来判断字符串是否与指定模式匹配
## isAscii - 用于判断字符串是否是 7 位 ASCII
## isJson - 确定给定的字符串是否是有效的 JSON
```python
def isJson(value) -> bool:
```

### - 参数说明

| 参数  | 类型 | 必选 | 默认值 | 说明 |
| ----- | ---- | ---- | ------ | ---- |
| value |      | Y    |        |      |

### - 使用示例

```python
Str.isJson('[1,2,3]')								# True
Str.isJson('{"first": "John", "last": "Doe"}')		# True
Str.isJson('{first: "John", last: "Doe"}')			# False
```



## isUrl - 确定给定值是否为有效 URL




## length - 获取字符个数

获取字符串中的字符个数，当遇到None时不会报错，返回`0`。

```python
def length(value, trim: bool = False) -> int:
```

### - 参数说

| 参数  | 类型 | 必选 | 默认值 | 说明             |
| ----- | ---- | ---- | ------ | ---------------- |
| value | str  | Y    |        | 字符串值         |
| trim  | bool | N    | False  | 是否去除前向空格 |

### - 参数说明

```python
# ASCII字符串：
Str.length('abcde')		# 结果：5

# 中文字符串：
Str.length('中文字符串')		# 结果：5

# 混合字符串：
Str.length('abcde中文字符串')	# 结果：10

# 非字符串值
Str.length(None)			# 结果： 0
```



## size - 获取字符串的字节个数

> utf-8编码：一个中文包含繁体字等于三个字节，一个英文字符等于一个字节。
>
> gbk编码：一个中文包含繁体字等于二个字节，一个英文字符等于一个字节。

```python
def size(cls, value, encoding: Optional[str] = None) -> int:
```

### - 参数说明

| 参数     | 类型          | 必选 | 默认值 | 说明                                          |
| -------- | ------------- | ---- | ------ | --------------------------------------------- |
| value    | str           | Y    |        | 字符串值                                      |
| encoding | Optional[str] | N    | None   | 字符串编码，默认当前环境默认编码，一般是utf-8 |

### - 使用示例

```python
from LuBan.helper import Str

print(f"ASCII字符串：{Str.size('abcde')}")		# 结果：5
print(f"中文字符串：{Str.size('中文字符串')}")		# 结果：15
print(f"中文字符串GBK：{Str.size('中文字符串', encoding='gbk')}")		# 结果：10
print(f"混合字符串：{Str.size('abcde中文字符串')}")					# 结果：20
print(f"混合字符串GBK：{Str.size('abcde中文字符串', encoding='gbk')}")		# 结果：15
print(f"非字符串值：{Str.size(None)}")		# 结果：0
```



## limit - 将字符串以指定长度进行截断

```python
def limit(cls, text, limit: int = 100, end: str = "...") -> str:
```

### - 参数说明

| 参数  | 类型 | 必选 | 默认值 | 说明         |
| ----- | ---- | ---- | ------ | ------------ |
| text  | str  | Y    |        | 字符串       |
| limit | int  | Y    | 100    | 限制最大长度 |
| end   | str  | N    | "..."  | 省略符       |

### - 使用示例

```python
from LuBan.helper import Str
import string

print(f"ASCII截取：{Str.limit(string.ascii_letters, 5)}")		   # 结果：abcde...
print(f"中文截取：{Str.limit('中文长度限制截取测试', 5)}")				# 结果：中文长度限...
print(f"中英文混合截取：{Str.limit('a中b文c的d长e度', 5)}")			# 结果：a中b文c...
print(f"非字符类型测试：{Str.limit(None, 2)}")						# 结果：No...
```



## words - 限制字符串中的单词数

## markdown
## inlineMarkdown
## mask - 使用重复的字符掩盖字符串的一部分
`mask`方法用重复字符掩盖字符串的一部分，并可用于混淆字符串段，例如电子邮件地址和电话号码。

```python
def mask(cls, text: str, index: int, length: Optional[int] = None, character: str = '*') -> str:
```

### - 参数说明

| 参数      | 类型      | 必选 | 默认值 | 说明                             |
| --------- | --------- | ---- | ------ | -------------------------------- |
| text      | str\|None | Y    |        | 字符串                           |
| index     | int       | Y    |        | 起始位置，可以使用负值           |
| length    | int       | N    | None   | 掩盖长度，若为负值则使用切片下标 |
| character | str       | N    | *      | 掩盖字符                         |

### - 使用示例

```python
from LuBan.helper import Str

_text = '0123456789'

# 从第5位开始遮掩
print(f"从第5位开始遮掩：{Str.mask(_text, 5)}")
# 结果：01234*****

# 从第3位开始，遮掩4位
print(f"从第3位开始，遮掩4位：{Str.mask(_text, 3, 4)}")
# 结果：012****789

# 从第1位至最后一位遮掩
print(f"从第1位至最后一位遮掩：{Str.mask(_text, 1, -1)}")
# 结果：0********9
```



## match - 返回字符串中和指定正则表达式匹配的部分

```python
def match(pattern: Union[str, re.Pattern], subject: str, flags: int = 0) -> str:
```

### - 参数说明

| 参数    | 类型                   | 必选 | 默认值 | 说明                                                         |
| ------- | ---------------------- | ---- | ------ | ------------------------------------------------------------ |
| pattern | Union[str, re.Pattern] | Y    |        | 匹配的正则表达式                                             |
| subject | str                    | Y    |        | 要匹配的字符串                                               |
| flags   | int                    | N    | 0      | 标志位，用于控制正则表达式的匹配方式，如：是否区分大小写，多行匹配等等 |

### - 使用示例

```python
Str.match('bar', 'foo bar')		# 结果：bar
Str.match('foo (.*)', 'foo bar')	# 结果：bar
```



## matchAll - 返回包含了字符串中与指定正则表达式匹配部分的集合
```python
def matchAll(pattern: Union[str, re.Pattern], subject: str, flags: int = 0) -> List[str]:
```

### - 参数说明

| 参数    | 类型                   | 必选 | 默认值 | 说明                                                         |
| ------- | ---------------------- | ---- | ------ | ------------------------------------------------------------ |
| pattern | Union[str, re.Pattern] | Y    |        | 匹配的正则表达式                                             |
| subject | str                    | Y    |        | 要匹配的字符串                                               |
| flags   | int                    | N    | 0      | 标志位，用于控制正则表达式的匹配方式，如：是否区分大小写，多行匹配等等 |

### - 使用示例

```python
Str.matchAll(r'bar', 'bar1 foo bar2')		# 结果：['bar', 'bar']
Str.matchAll(r'f(\w*)', 'bar fun bar fly') 	# 结果：['un', 'ly']
```



## isMatch - 用于判断给定的字符串是否与正则表达式匹配

```python
def isMatch(pattern: Union[str, re.Pattern, List[str], Tuple[str], List[re.Pattern], Tuple[re.Pattern]], subject: str, flags: int = 0) -> bool:
```

### - 参数说明

| 参数    | 类型                                                         | 必选 | 默认值 | 说明                                                         |
| ------- | ------------------------------------------------------------ | ---- | ------ | ------------------------------------------------------------ |
| pattern | Union[str, re.Pattern, List[str], Tuple[str], List[re.Pattern], Tuple[re.Pattern]] | Y    |        | 匹配的正则表达式，可批量测试                                 |
| subject | str                                                          | Y    |        | 要匹配的字符串                                               |
| flags   | int                                                          | N    | 0      | 标志位，用于控制正则表达式的匹配方式，如：是否区分大小写，多行匹配等等 |

### - 使用示例

```python
Str.isMatch('foo (.*)', 'foo bar')		# 结果：True
Str.isMatch('foo (.*)', 'laravel')		# 结果：False
```



## padBoth - 在指定字符串的两侧填充上另一字符串

```python
def padBoth(value: str, length: int, pad: str = ' ') -> str:
```

### - 参数说明

| 参数   | 类型 | 必选 | 默认值 | 说明                 |
| ------ | ---- | ---- | ------ | -------------------- |
| value  | str  | Y    |        | 字符串               |
| length | int  | Y    |        | 要求填充字符串总长度 |
| pad    | str  | N    | ' '    | 填充的字符           |

### - 使用示例

```python
Str.padBoth('James', 10, '_')			# '__James___'
Str.padBoth('James', 10)				# '  James   '
```



## padLeft - 在指定字符串的左侧填充上另一字符串

```python
def padLeft(value: str, length: int, pad: str = ' ') -> str:
```

### - 参数说明

| 参数   | 类型 | 必选 | 默认值 | 说明                 |
| ------ | ---- | ---- | ------ | -------------------- |
| value  | str  | Y    |        | 字符串               |
| length | int  | Y    |        | 要求填充字符串总长度 |
| pad    | str  | N    | ' '    | 填充的字符           |

### - 使用示例



## padRight - 在指定字符串的右侧填充上另一字符串

```python
def padRight(value: str, length: int, pad: str = ' ') -> str:
```

### - 参数说明

| 参数   | 类型 | 必选 | 默认值 | 说明                 |
| ------ | ---- | ---- | ------ | -------------------- |
| value  | str  | Y    |        | 字符串               |
| length | int  | Y    |        | 要求填充字符串总长度 |
| pad    | str  | N    | ' '    | 填充的字符           |

### - 使用示例



## parseCallback


## plural - 将单数形式的字符串转换为复数形式

```python
def plural(word: str) -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明           |
| ---- | ---- | ---- | ------ | -------------- |
| word | str  | Y    |        | 需要转换的单词 |

### - 使用示例

```python
Str.plural('car')			# cars
Str.plural('cars')			# cars
Str.plural('child')			# children
Str.plural('children')		# children
```



## pluralStudly - 将以驼峰格式的单数字符串转化为其复数形式

## singular - 将字符串转换为其单数形式
```python
def singular(word: str) -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明           |
| ---- | ---- | ---- | ------ | -------------- |
| word | str  | Y    |        | 需要转换的单词 |

### - 使用示例

```python
Str.singular('car')				# car
Str.singular('cars')			# car
Str.singular('child')			# child
Str.singular('children')		# child
```



## password - 生成给定长度的安全随机密码

`password` 方法可用于生成给定长度的安全随机密码。密码由字母、数字、符号和空格组成。默认情况下，密码长度为 32 位

```python
def password(cls, length: int = 32, letters: bool = True, numbers: bool = True, symbols: bool = True, spaces: bool = False) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明                 |
| ------- | ---- | ---- | ------ | -------------------- |
| length  | int  | N    | 32     | 生成密码长度，默认32 |
| letters | bool | N    | True   | 是否必须包含字母     |
| numbers | bool | N    | True   | 是否必须包含数字     |
| symbols | bool | N    | True   | 是否必须包含符号     |
| spaces  | bool | N    | False  | 是否必须包含空格     |

### - 使用示例

```python
Str.password()		# '&2kNA1*)fF|3GJ{&X?_;8&GS-x9-\St['
Str.password(12)	# '5f{SPSKh?|!G'
```



## position - 查找字符串在另一字符串中第一次出现的位置

`position`返回字符串在另一字符串中第一次出现的位置，如果没有找到字符串则返回 -1

```python
def position(haystack: str, needle: str, caseSensitive: bool = True) -> int:
```

### - 参数说明

| 参数          | 类型 | 必选 | 默认值 | 说明                             |
| ------------- | ---- | ---- | ------ | -------------------------------- |
| haystack      | str  | Y    |        | 被搜索的字符串                   |
| needle        | str  | Y    |        | 要查找的字符串                   |
| caseSensitive | bool | N    | True   | 是否大小写母感，默认为区分大小写 |

### - 使用示例

```python
Str.position('You love python, I love python too!', 'python')		# 9
Str.position('You love python, I love python too!', 'php')			# -1
```



## positionLast - 查找字符串在另一字符串中最后一次出现的位置

`positionLast`查找字符串在另一字符串中最后一次出现的位置，如果没有找到字符串则返回 -1

```python
def positionLast(haystack: str, needle: str, caseSensitive: bool = True) -> int:
```

### - 参数说明

| 参数          | 类型 | 必选 | 默认值 | 说明                             |
| ------------- | ---- | ---- | ------ | -------------------------------- |
| haystack      | str  | Y    |        | 被搜索的字符串                   |
| needle        | str  | Y    |        | 要查找的字符串                   |
| caseSensitive | bool | N    | True   | 是否大小写母感，默认为区分大小写 |

### - 使用示例

```python
Str.position('You love python, I love python too!', 'python')		# 24
Str.position('You love python, I love python too!', 'php')			# -1
```



## random - 生成指定长度的随机字符串

获取指定长度的随机字母数字组合的字符串

```python
def random(cls, length: int = 32, charType: int = 1, expand: str = '') -> str:
```

### - 参数说明

| 参数     | 类型 | 必选 | 默认值 | 说明                       |
| -------- | ---- | ---- | ------ | -------------------------- |
| length   | int  | Y    | 32     | 生成字符串长度             |
| charType | int  | Y    | 1      | 字符串组成类型，默认纯字母 |
| expand   | str  | N    | ""     | （可选）自定义扩展字符串   |

#### - charType 可选

* CHAR_TYPE_DIGITS  纯数字
* CHAR_TYPE_ALPHA  纯字母
* CHAR_TYPE_ALPHA_NUM  字母和数字
* CHAR_TYPE_ALPHA_DASH  字母、数字、下划线，中划线
* CHAR_TYPE_ALPHA_CHS  中文

### - 使用示例

```python
# 默认生成纯字母
Str.random()	# 结果：lZhHZulLprwqiukulTPvVNfkgEULCeqF

# 纯数字
Str.random(16, charType=Str.CHAR_TYPE_DIGITS)	# 结果：3111549986706968

# 字母和数字
Str.random(charType=Str.CHAR_TYPE_ALPHA_NUM) # 结果：aAs9v9kBlCPhmI8TVXeW2kU4uaHOHvr7

# 字母、数字、下划线，中划线
Str.random(charType=Str.CHAR_TYPE_ALPHA_DASH) # 结果：luJXh3r_3Tmgcl00jwH6_lrT-oOxxItb

# 中文
Str.random(length=4, charType=Str.CHAR_TYPE_ALPHA_CHS)	# 结果：集员地断
```



## toStringOr


## replace - 用于替换字符串中的给定字符串

`replace` 方法用于将字符串中的指定字符串替换为另一指定字符串

```python
def replace(cls, subject: str, search: str, replace: str, count: int = 0, caseSensitive: bool = True) -> str:
```

### - 参数说明

| 参数          | 类型 | 必选 | 默认值 | 说明                                |
| ------------- | ---- | ---- | ------ | ----------------------------------- |
| subject       | str  | Y    |        | 要搜索替换的目标字符串              |
| search        | str  | Y    |        | 要查找的值                          |
| replace       | str  | Y    |        | 替换 `search` 的值                  |
| count         | int  | N    | 0      | 替换的最大次数，默认是`0`（无限制） |
| caseSensitive | bool | N    | True   | 区分大小写，默认`True`区分          |

### - 使用示例

默认区分大小写

```python
# ASCII替换，默认区分大小写
Str.replace('abABabABabAB', 'ab', 'ef')		# 结果：efABefABefAB

# 中文替换
Str.replace('中文中文中文', '中', '英')			# 结果：英文英文英文

# 限制最大替换2次
Str.replace('abABabABabAB', 'ab', 'ef', 2)		# 结果：efABefABabAB
Str.replace('中文中文中文', '中', '英', 2)		   # 结果：英文英文中文
```

强制忽略大小写

```python
# ASCII替换，忽略大小写
Str.replace('abABabABabAB', 'ab', 'ef', caseSensitive=False)	# 结果：efefefefefef

# 限制最大替换2次
Str.replace('abABabABabAB', 'ab', 'ef', 2)		# 结果：efABefABabAB
Str.replace('abABabABabAB', 'ab', 'ef', 2, caseSensitive=False) # 结果：efefabABabAB
```



## replaceIgnoreCase - 用于替换字符串中的给定字符串（不区分大小写）

```python
def replaceIgnoreCase(cls, subject: str, search: str, replace: str, count: int = 0) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明                                |
| ------- | ---- | ---- | ------ | ----------------------------------- |
| subject | str  | Y    |        | 要搜索替换的目标字符串              |
| search  | str  | Y    |        | 要查找的值                          |
| replace | str  | Y    |        | 替换 `search` 的值                  |
| count   | int  | N    | 0      | 替换的最大次数，默认是`0`（无限制） |

### - 使用示例



## replaceArray - 使用数组有序的替换字符串中的特定字符

```python
def replaceArray(subject: str, search: str, replace: Union[List[str], Tuple[str]]) -> str:
```

### - 参数说明

| 参数    | 类型                         | 必选 | 默认值 | 说明             |
| ------- | ---------------------------- | ---- | ------ | ---------------- |
| subject | str                          | Y    |        | 字符串           |
| search  | str                          | Y    |        | 需要替换的字符串 |
| replace | Union[List[str], Tuple[str]] | Y    |        | 替换的字符串序列 |

### - 使用示例

```python
Str.replaceArray('该活动将在 ? 至 ? 举行', '?', ['8:30', '9:00'])
# 该活动将在 8:30 至 9:00 举行
```



## replaceFirst - 替换字符串中给定值的第一个匹配项

```python
def replaceFirst(cls, subject: str, search: str, replace: str) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明             |
| ------- | ---- | ---- | ------ | ---------------- |
| subject | str  | Y    |        | 字符串           |
| search  | str  | Y    |        | 需要替换的字符串 |
| replace | str  | Y    |        | 替换的字符串     |

### - 使用示例

```python
Str.replaceFirst('the quick brown fox jumps over the lazy dog', 'the', 'a')
# a quick brown fox jumps over the lazy dog
```



## replaceLast - 替换字符串中最后一次出现的给定值

```python
def replaceLast(cls, subject: str, search: str, replace: str) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明             |
| ------- | ---- | ---- | ------ | ---------------- |
| subject | str  | Y    |        | 字符串           |
| search  | str  | Y    |        | 需要替换的字符串 |
| replace | str  | Y    |        | 替换的字符串     |

### - 使用示例

```python
Str.replaceLast('the quick brown fox jumps over the lazy dog', 'the', 'a')
# the quick brown fox jumps over a lazy dog
```



## replaceStart - 替换字符串开头第一个出现的给定值

```python
def replaceStart(cls, subject: str, search: str, replace: str) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明             |
| ------- | ---- | ---- | ------ | ---------------- |
| subject | str  | Y    |        | 字符串           |
| search  | str  | Y    |        | 需要替换的字符串 |
| replace | str  | Y    |        | 替换的字符串     |

### - 使用示例



## replaceEnd - 如果给定值出现在字符串末尾，则替换最后出现的值

```python
def replaceEnd(cls, subject: str, search: str, replace: str) -> str:
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明             |
| ------- | ---- | ---- | ------ | ---------------- |
| subject | str  | Y    |        | 字符串           |
| search  | str  | Y    |        | 需要替换的字符串 |
| replace | str  | Y    |        | 替换的字符串     |

### - 使用示例



## replaceMatches - 用给定的替换字符串替换与模式匹配的字符串的所有部分

```python
def replaceMatches(subject, pattern: Union[str, re.Pattern], replace: Union[str, Callable], count: int = -1, flags: int = 0):
```

### - 参数说明

| 参数    | 类型 | 必选 | 默认值 | 说明                                                         |
| ------- | ---- | ---- | ------ | ------------------------------------------------------------ |
| subject | str  | Y    |        | 要被查找替换的原始字符串                                     |
| pattern | str  | Y    |        | 要搜索的模式，可以是字符串                                   |
| replace | str  | Y    |        | 替换的字符串，也可为一个函数                                 |
| count   | int  | N    | 0      | 可选，对于每个模式用于每个 subject 字符串的最大可替换次数。 默认是0（无限制） |
| flags   | bool | N    | True   | 标志位，用于控制正则表达式的匹配方式，如：是否区分大小写，多行匹配等等 |

### - 使用示例

```python
Str.replaceMatches('(+1) 501-555-1000', '[^A-Za-z0-9]+', '')		# 15015551000
```



## substrReplace - 替换字符串一部分中的文本

`substrReplace` 方法替换字符串一部分中的文本，从第三个参数指定的位置开始，替换第四个参数指定的字符数。 当「0」传递给方法的第四个参数将在指定位置插入字符串，而不是替换字符串中的任何现有字符

```python
def substrReplace(subject: str, replace: str, offset=0, length: Optional[int] = None) -> str:
```

### - 参数说明

| 参数    | 类型          | 必选 | 默认值 | 说明                                                         |
| ------- | ------------- | ---- | ------ | ------------------------------------------------------------ |
| subject | str           | Y    |        | 被检查的字符串                                               |
| replace | str           | Y    |        | 要替换或插入的字符串                                         |
| offset  | int           | N    | 0      | 在字符串中何处开始搜索<br />正数 - 在字符串中的指定位置开始替换<br/>负数 - 在从字符串结尾的指定位置开始替换<br/>0 - 在字符串中的第一个字符处开始替换 |
| length  | Optional[int] | N    | None   | 要替换多少个字符。默认是与字符串长度相同<br />正数 - 被替换的字符串长度<br/>负数 - 表示待替换的子字符串结尾处距离 string 末端的字符个数。<br/>0 - 插入而非替换 |

### - 使用示例

```python
Str.substrReplace('Hello world', 'Shanghai', 6)		# 'Hello Shanghai'
Str.substrReplace('1300', ':', 2)					# '13:'
Str.substrReplace('1300', ':', 2, 0)				# '13:00'
```



## swap - 替换给定字符串中的多个值

```python
def swap(maps: Dict[str, str], subject: str) -> str:
```

### - 参数说明

| 参数    | 类型           | 必选 | 默认值 | 说明             |
| ------- | -------------- | ---- | ------ | ---------------- |
| maps    | Dict[str, str] | Y    |        | 替换的映射字典   |
| subject | str            | Y    |        | 需要替换的字符串 |

### - 使用示例

```python
Str.swap({
        'Tacos': 'Burritos',
        'great': 'fantastic'
    }, 'Tacos are great!')

# 结果：Burritos are fantastic!
```



## prepend - 用于在指定字符串的开头插入另一指定字符串

## append - 将给定的值附加到字符串
## remove - 用于从字符串中删除给定的值或值数组
`remove` 方法从字符串中删除给定值或给定数组内的所有值，还可以将 `False`作为第三个参数传递给 `remove` 方法以在删除字符串时忽略大小写。

```python
def remove(search: Union[str, Tuple[str], List[str], Set[str]], subject: str, caseSensitive: bool = True) -> str:
```

### - 参数说明

| 参数          | 类型                                        | 必选 | 默认值 | 说明                             |
| ------------- | ------------------------------------------- | ---- | ------ | -------------------------------- |
| search        | Union[str, Tuple[str], List[str], Set[str]] | Y    |        | 执行替换的数组或者字符串         |
| subject       | str                                         | Y    |        | 执行替换的数组或者字符串         |
| caseSensitive | bool                                        | N    | True   | 是否大小写敏感，默认为区分大小写 |

### - 使用示例

```python
Str.remove('e', 'Peter Piper picked a peck of pickled peppers.')
# 结果：Ptr Pipr pickd a pck of pickld ppprs.

Str.remove(['e', 'p'], 'Peter Piper picked a peck of pickled peppers.')
# 结果：Ptr Pir ickd a ck of ickld rs.

Str.remove(['e', 'p'], 'Peter Piper picked a peck of pickled peppers.', False)
# 结果：tr ir ickd a ck of ickld rs.
```



## reverse - 反转给定的字符串

```python
def reverse(value: str) -> str:
```

### - 参数说明

| 参数  | 类型 | 必选 | 默认值 | 说明   |
| ----- | ---- | ---- | ------ | ------ |
| value | str  | Y    |        | 字符串 |

### - 使用示例

```python
Str.reverse('Hello World 中文')		# 结果：文中 dlroW olleH
```



## startsWith - 确定给定字符串是否以给定值开头

`startsWith` 方法用来判断给定的字符串是否为给定值的开头，如果传递了一个可能值的数组且字符串以任何给定值开头，则 `startsWith` 方法将返回 `True`

```python
def startsWith(cls, haystack: str, needles: Union[str, List[str], Tuple[str], Set[str]], caseSensitive: bool = True) -> bool:
```

### - 参数说明

| 参数          | 类型                                        | 必选 | 默认值 | 说明                             |
| ------------- | ------------------------------------------- | ---- | ------ | -------------------------------- |
| haystack      | str                                         | Y    |        | 要被检查的 string                |
| needles       | Union[str, List[str], Tuple[str], Set[str]] | Y    |        | 前缀字符串或集合                 |
| caseSensitive | bool                                        | N    | True   | 是否大小写敏感，默认为区分大小写 |

### - 使用示例

```python
Str.startsWith('This is my name', 'This')						# 结果： True
Str.startsWith('This is my name', 'this')						# 结果： False	
Str.startsWith('This is my name', 'this', False)				# 结果： True
Str.startsWith('This is my name', ['This', 'That', 'There'])	# 结果： True
```



## endsWith - 用于判断指定字符串是否以另一指定字符串结尾

endsWith 方法确定给定字符串是否以给定值结尾，还可以传递一个值数组来确定给定字符串是否以数组中的任何值结尾。

```python
def endsWith(cls, haystack: str, needles: Union[str, List[str], Tuple[str], Set[str]], caseSensitive: bool = True) -> bool:
```

### - 参数说明

| 参数          | 类型                                        | 必选 | 默认值 | 说明                             |
| ------------- | ------------------------------------------- | ---- | ------ | -------------------------------- |
| haystack      | str                                         | Y    |        | 要被检查的 string                |
| needles       | Union[str, List[str], Tuple[str], Set[str]] | Y    |        | 结尾字符串或集合                 |
| caseSensitive | bool                                        | N    | True   | 是否大小写敏感，默认为区分大小写 |

### - 使用示例

```python
Str.endsWith('This is my name', 'name')							# 结果： True
Str.endsWith('This is my name', 'Name')							# 结果： False
Str.endsWith('This is my name', 'Name', False)					# 结果： True
Str.endsWith('This is my name', ['This', 'foo', 'Name'])		# 结果： False
```



## start - 将给定的值添加到字符串的开始位置

`start` 方法将给定值的单个实例添加到字符串中，前提是该字符串尚未以该值开头

```python
def start(value: str, prefix: str) -> str:
```

### - 参数说明

| 参数          | 类型 | 必选 | 默认值 | 说明                             |
| ------------- | ---- | ---- | ------ | -------------------------------- |
| text          | str  | Y    |        | 要被检查的 string                |
| prefix        | str  | Y    |        | 指定字符前缀                     |
| caseSensitive | bool | N    | True   | 是否大小写母感，默认为区分大小写 |

### - 使用示例

```python
Str.start('this/string', '/')		# 结果：/this/string
Str.start('/this/string', '/')		# 结果：/this/string
```



## finish - 将指定的字符串修改为以指定的值结尾的形式

`finish` 方法将给定值的单个实例添加到字符串中（如果它尚未以该值结尾）

```python
def finish(value: str, cap: str) -> str:
```

### - 参数说明

| 参数          | 类型 | 必选 | 默认值 | 说明                             |
| ------------- | ---- | ---- | ------ | -------------------------------- |
| text          | str  | Y    |        | 要被检查的 string                |
| cap           | str  | Y    |        | 指定结尾字符                     |
| caseSensitive | bool | N    | True   | 是否大小写母感，默认为区分大小写 |

### - 使用示例

```python
Str.finish('this/string', '/')		# 结果：this/string/
Str.finish('this/string/', '/')		# 结果：this/string/
```



## lower - 用于将字符串转换为小写

```python
def lower(value) -> str:
```

### - 参数说明

| 参数  | 类型 | 必选 | 默认值 | 说明   |
| ----- | ---- | ---- | ------ | ------ |
| value | str  | Y    | 无     | 字符串 |

### - 使用示例



## upper - 将给定字符串转换为大写

```python
def upper(value) -> str:
```

### - 参数说明

| 参数  | 类型 | 必选 | 默认值 | 说明   |
| ----- | ---- | ---- | ------ | ------ |
| value | str  | Y    | 无     | 字符串 |

### - 使用示例



## headline - 将给定字符串的每个单词转换为标题大小写

`headline` 方法会将由大小写、连字符或下划线分隔的字符串转换为空格分隔的字符串，每个单词的首字母大写

```python
def headline(cls, text: str) -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明   |
| ---- | ---- | ---- | ------ | ------ |
| text | str  | Y    |        | 字符串 |

### - 使用示例

```python
Str.headline('steve_jobs')
# Steve Jobs

Str.headline('EmailNotificationDelivery')
# Email Notification Delivery
```



## title - 将给定的字符串转换为 `Title Case`
```python
def title(value: str) -> str:
```

### - 参数说明

| 参数  | 类型 | 必选 | 默认值 | 说明   |
| ----- | ---- | ---- | ------ | ------ |
| value | str  | Y    | 无     | 字符串 |

### - 使用示例：

```python
_text = "They're john's relatives."

# Python str.title()方法存在的问题：
_text.title()
# 结果： They'Re John'S Relatives.

# 使用Str.title()方法
Str.title(_text)
# 结果： They're John's Relatives.
```



## slug - 从给定字符串生成 URL 友好的 `“slug”`

## camel - 将指定字符串转换为`camelCase 驼峰式` 表示方法
```python
def camel(cls, text: str) -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明   |
| ---- | ---- | ---- | ------ | ------ |
| text | str  | Y    |        | 字符串 |

### - 使用示例

```python
Str.camel('foo_bar')		# fooBar
```



## studly - 将给定字符串转换为 `StudlyCase`

```python
def studly(cls, value: str) -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明   |
| ---- | ---- | ---- | ------ | ------ |
| text | str  | Y    |        | 字符串 |

### - 使用示例

```python
Str.studly('foo_bar')			# FooBar
```



## snake - 法将给定字符串转换为 `snake_case`

```python
def snake(cls, text: str, delimiter: str = '_') -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明   |
| ---- | ---- | ---- | ------ | ------ |
| text | str  | Y    |        | 字符串 |
| sep  | str  | N    | _      | "_"    |

### - 使用示例

```python
Str.snake('fooBar')				
# foo_bar
```



## kebab - 将字符串转换为烤串式（ `kebab-case` ）表示方法

```python
def kebab(cls, text: str) -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明   |
| ---- | ---- | ---- | ------ | ------ |
| text | str  | Y    |        | 字符串 |

### - 使用示例

```python
Str.kebab("fooBar")
# foo-bar
```



## squish - 删除字符串中所有无关紧要的空白，包括字符串之间的空白

```python
def squish(text: str) -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明   |
| ---- | ---- | ---- | ------ | ------ |
| text | str  | Y    |        | 字符串 |

### - 使用示例

```python
Str.squish('    Hello    Python    中文     世界')			# Hello Python 中文 世界
```



## ucfirst - 返回第一个字符大写的给定字符串

```python
def ucfirst(text: str) -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明   |
| ---- | ---- | ---- | ------ | ------ |
| text | str  | Y    |        | 字符串 |

### - 使用示例

```python
Str.ucfirst('foo bar')

# Foo bar
```



## lcfirst - 返回给定的字符串的第一个字符为小写字母

```python
def lcfirst(text: str) -> str:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明   |
| ---- | ---- | ---- | ------ | ------ |
| text | str  | Y    |        | 字符串 |

### - 使用示例

```python
Str.lcfirst('Foo Bar')

# foo Bar
```



## substrCount - 返回给定字符串中给定值的出现次数
```python
def substrCount(haystack: str, needle: str, offset: int = 0, length: Optional[int] = None) -> int:
```

### - 参数说明

| 参数     | 类型          | 必选 | 默认值 | 说明                   |
| -------- | ------------- | ---- | ------ | ---------------------- |
| haystack | str           | Y    |        | 被检查的字符串         |
| needle   | str           | Y    |        | 要搜索的字符串         |
| offset   | int           | N    | 0      | 在字符串中何处开始搜索 |
| length   | Optional[int] | N    | None   | 搜索的长度             |

### - 使用示例

```python
Str.substrCount('If you like ice cream, you will like snow cones.', 'like')		# 结果：2
```



## take

## ucsplit - 将给定的字符串按大写字符拆分为数组
```python
def ucsplit(text: str) -> List[str]:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明   |
| ---- | ---- | ---- | ------ | ------ |
| text | str  | Y    |        | 字符串 |

### - 使用示例

```python
Str.ucsplit('FooBar')
# ['Foo', 'Bar']

Str.ucsplit('Foo Bar')
# ['Foo', 'Bar']

Str.ucsplit('TheLongAndWindingRoad')
# ['The', 'Long', 'And', 'Winding', 'Road']

Str.ucsplit('TheLongAndWindingRoad ABC A123B45')
# ['The', 'Long', 'And', 'Winding', 'Road', 'A', 'B', 'C', 'A123', 'B45']
```



## wordCount - 返回字符串包含的单词数

## wordWrap
## uuid - 生成一个 UUID（版本 4）

Python UUID模块支持以下版本的UUID：

- UUID1 –使用主机MAC地址，序列号和当前时间生成UUID。此版本使用IEEE 802 MAC地址。
- UUID3和UUID 5使用加密哈希和应用程序提供的文本字符串来生成UUID。UUID 3使用MD5哈希，而UUID 5使用SHA-1哈希。
- UUID4使用伪随机数生成器生成UUID。

```python
def uuid() -> str:
```

### - 参数说明

无

### - 使用示例

```python
for _ in range(10):
	print(Str.uuid())
	
# 生成结果：
8517ebfb-8aba-4fbd-9d29-9b2961e51314
33cda797-19be-4f3e-85cd-f37c40b68803
7ca1e4e2-23fb-439b-8fb0-f4b002339d26
72f10ee6-91a7-4ef1-b4e4-4ddd10597ca0
9bdce14b-fec5-468d-abb1-701c46cc9835
039d8897-9846-4709-a165-b0f1e95baeda
f30e00a4-2ddb-459f-b121-efe05d9d70fb
74c645a5-d77f-4f38-8d48-ebe9373f4c87
c388a92e-5dc3-43cd-ac05-cfba0a5a8640
8e90d7d9-ff64-4a49-9452-d9d41981a410
```



## orderedUuid - 用于生成一个「时间戳优先」的 UUID 

## isUuid - 确定给定的字符串是否是一个 UUID
## ulid - 生成一个 ULID
## isUlid - 确定给定的字符串是否一个 ULID


## isEmpty - 确定给定的字符串是否为空

判断字符串是否为空，可判断None值和去除前后空格。

```python
def isEmpty(val, trim: bool = True) -> bool:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明             |
| ---- | ---- | ---- | ------ | ---------------- |
| val  | str  | Y    | 无     | 字符串值         |
| trim | bool | N    | False  | 是否去除前向空格 |

### - 使用示例



## isNotEmpty - 确定给定的字符串是否不为空

判断字符串是否为非空，可判断None值和去除前后空格。

```python
def isNotEmpty(val, trim: bool = False) -> bool:
```

### - 参数说明

| 参数 | 类型 | 必选 | 默认值 | 说明             |
| ---- | ---- | ---- | ------ | ---------------- |
| val  | str  | Y    | 无     | 字符串值         |
| trim | bool | N    | False  | 是否去除前向空格 |

### - 使用示例



## flushCache



