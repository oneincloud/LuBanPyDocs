# Str - 字符串

## TODO功能清单：

- [ ] after - 返回字符串中指定值之后的所有内容
- [ ] afterLast - 返回字符串中指定值最后一次出现后的所有内容
- [ ] ascii - 尝试将字符串转换为 ASCII 值
- [ ] transliterate
- [ ] before - 返回字符串中指定值之前的所有内容
- [ ] beforeLast - 返回字符串中指定值最后一次出现前的所有内容
- [ ] between - 返回字符串在指定两个值之间的内容
- [ ] betweenFirst - 返回字符串在指定两个值之间的最小可能的部分
- [ ] charAt
- [ ] contains - 判断指定字符串中是否包含另一指定字符串
- [ ] containsAll - 用于判断指定字符串是否包含指定数组中的所有值
- [ ] convertCase
- [ ] excerpt - 提取字符串中给定短语匹配到的第一个片段
- [ ] wrap
- [ ] is - 用来判断字符串是否与指定模式匹配
- [ ] isAscii - 用于判断字符串是否是 7 位 ASCII
- [ ] isJson - 确定给定的字符串是否是有效的 JSON
- [ ] isUrl
- [ ] length - 返回指定字符串的长度
- [ ] limit - 将字符串以指定长度进行截断
- [ ] words - 限制字符串中的单词数
- [ ] markdown
- [ ] inlineMarkdown
- [ ] mask - 使用重复的字符掩盖字符串的一部分
- [ ] match - 返回字符串中和指定正则表达式匹配的部分
- [ ] isMatch - 用于判断给定的字符串是否与正则表达式匹配
- [ ] matchAll - 返回包含了字符串中与指定正则表达式匹配部分的集合
- [ ] padBoth - 在指定字符串的两侧填充上另一字符串
- [ ] padLeft - 在指定字符串的左侧填充上另一字符串
- [ ] padRight - 在指定字符串的右侧填充上另一字符串
- [ ] parseCallback
- [ ] plural - 将单数形式的字符串转换为复数形式
- [ ] pluralStudly - 将以驼峰格式的单数字符串转化为其复数形式
- [ ] singular - 将字符串转换为其单数形式
- [ ] password - 生成给定长度的安全随机密码
- [ ] position
- [x] random - 生成指定长度的随机字符串
- [ ] repeat
- [ ] toStringOr
- [ ] replace - 用于替换字符串中的给定字符串
- [ ] replaceArray - 使用数组有序的替换字符串中的特定字符
- [ ] replaceFirst - 替换字符串中给定值的第一个匹配项
- [ ] replaceLast - 替换字符串中最后一次出现的给定值
- [ ] replaceStart
- [ ] replaceEnd
- [ ] replaceMatches - 用给定的替换字符串替换与模式匹配的字符串的所有部分
- [ ] substrReplace - 替换字符串一部分中的文本
- [ ] swap - 替换给定字符串中的多个值
- [ ] prepend - 用于在指定字符串的开头插入另一指定字符串
- [ ] append - 将给定的值附加到字符串
- [ ] remove - 用于从字符串中删除给定的值或值数组
- [ ] reverse - 反转给定的字符串
- [ ] start - 给定值的单个实例添加到字符串中
- [ ] finish - 将指定的字符串修改为以指定的值结尾的形式
- [ ] lower - 用于将字符串转换为小写
- [ ] upper - 将给定字符串转换为大写
- [ ] headline - 将由大小写、连字符或下划线分隔的字符串转换为空格分隔的字符串，每个单词的首字母大写
- [ ] title - 将给定的字符串转换为 `Title Case`
- [ ] slug - 从给定字符串生成 URL 友好的 `“slug”`
- [ ] camel - 将指定字符串转换为`camelCase 驼峰式` 表示方法
- [ ] snake - 法将给定字符串转换为 `snake_case`
- [ ] studly - 将给定字符串转换为 `StudlyCase`
- [ ] kebab - 将字符串转换为烤串式（ `kebab-case` ）表示方法
- [ ] squish - 删除字符串中所有无关紧要的空白，包括字符串之间的空白
- [ ] ucfirst - 返回第一个字符大写的给定字符串
- [ ] lcfirst - 返回给定的字符串的第一个字符为小写字母
- [ ] startsWith - 确定给定字符串是否以给定值开头
- [ ] endsWith - 用于判断指定字符串是否以另一指定字符串结尾
- [ ] substr - 类似python字符串的`切片`功能
- [ ] substrCount - 返回给定字符串中给定值的出现次数
- [ ] take
- [ ] ucsplit - 将给定的字符串按大写字符拆分为数组
- [ ] wordCount - 返回字符串包含的单词数
- [ ] wordWrap
- [ ] uuid - 生成一个 UUID（版本 4）
- [ ] orderedUuid - 用于生成一个「时间戳优先」的 UUID 
- [ ] isUuid - 确定给定的字符串是否是一个 UUID
- [ ] ulid - 生成一个 ULID
- [ ] isUlid - 确定给定的字符串是否一个 ULID
- [x] isEmpty - 确定给定的字符串是否为空
- [x] isNotEmpty - 确定给定的字符串是否不为空
- [ ] flushCache






## after - 返回字符串中指定值之后的所有内容
## afterLast - 返回字符串中指定值最后一次出现后的所有内容
## ascii - 尝试将字符串转换为 ASCII 值
## transliterate
## before - 返回字符串中指定值之前的所有内容
## beforeLast - 返回字符串中指定值最后一次出现前的所有内容
## between - 返回字符串在指定两个值之间的内容
## betweenFirst - 返回字符串在指定两个值之间的最小可能的部分
## charAt
## contains - 判断指定字符串中是否包含另一指定字符串
## containsAll - 用于判断指定字符串是否包含指定数组中的所有值
## convertCase
## excerpt - 提取字符串中给定短语匹配到的第一个片段
## wrap
## is - 用来判断字符串是否与指定模式匹配
## isAscii - 用于判断字符串是否是 7 位 ASCII
## isJson - 确定给定的字符串是否是有效的 JSON
## isUrl
## length - 返回指定字符串的长度
## limit - 将字符串以指定长度进行截断
## words - 限制字符串中的单词数
## markdown
## inlineMarkdown
## mask - 使用重复的字符掩盖字符串的一部分
## match - 返回字符串中和指定正则表达式匹配的部分
## isMatch - 用于判断给定的字符串是否与正则表达式匹配
## matchAll - 返回包含了字符串中与指定正则表达式匹配部分的集合
## padBoth - 在指定字符串的两侧填充上另一字符串
## padLeft - 在指定字符串的左侧填充上另一字符串
## padRight - 在指定字符串的右侧填充上另一字符串
## parseCallback
## plural - 将单数形式的字符串转换为复数形式
## pluralStudly - 将以驼峰格式的单数字符串转化为其复数形式
## singular - 将字符串转换为其单数形式
## password - 生成给定长度的安全随机密码
## position


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





## repeat

## toStringOr
## replace - 用于替换字符串中的给定字符串
## replaceArray - 使用数组有序的替换字符串中的特定字符
## replaceFirst - 替换字符串中给定值的第一个匹配项
## replaceLast - 替换字符串中最后一次出现的给定值
## replaceStart
## replaceEnd
## replaceMatches - 用给定的替换字符串替换与模式匹配的字符串的所有部分
## substrReplace - 替换字符串一部分中的文本
## swap - 替换给定字符串中的多个值
## prepend - 用于在指定字符串的开头插入另一指定字符串
## append - 将给定的值附加到字符串
## remove - 用于从字符串中删除给定的值或值数组
## reverse - 反转给定的字符串
## start - 给定值的单个实例添加到字符串中
## finish - 将指定的字符串修改为以指定的值结尾的形式
## lower - 用于将字符串转换为小写
## upper - 将给定字符串转换为大写
## headline - 将由大小写、连字符或下划线分隔的字符串转换为空格分隔的字符串，每个单词的首字母大写
## title - 将给定的字符串转换为 `Title Case`
## slug - 从给定字符串生成 URL 友好的 `“slug”`
## camel - 将指定字符串转换为`camelCase 驼峰式` 表示方法
## snake - 法将给定字符串转换为 `snake_case`
## studly - 将给定字符串转换为 `StudlyCase`
## kebab - 将字符串转换为烤串式（ `kebab-case` ）表示方法
## squish - 删除字符串中所有无关紧要的空白，包括字符串之间的空白
## ucfirst - 返回第一个字符大写的给定字符串
## lcfirst - 返回给定的字符串的第一个字符为小写字母
## startsWith - 确定给定字符串是否以给定值开头
## endsWith - 用于判断指定字符串是否以另一指定字符串结尾
## substr - 类似python字符串的`切片`功能
## substrCount - 返回给定字符串中给定值的出现次数
## take
## ucsplit - 将给定的字符串按大写字符拆分为数组
## wordCount - 返回字符串包含的单词数
## wordWrap
## uuid - 生成一个 UUID（版本 4）
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



