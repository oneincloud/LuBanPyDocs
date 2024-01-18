# Hash - 组件：哈希计算辅助工具

## TODO功能清单：

- [ ] hash - 计算字符串 哈希 值
- [ ] fileHash - 计算文件 哈希 值
- [ ] Hash实例使用

### 快捷方法

- [ ] md5 - 计算字符串的 MD5 散列

- [ ] sha1 - 计算字符串的 SHA-1 散列

- [ ] sha224 - 计算字符串的 SHA-224 散列

- [ ] sha256 - 计算字符串的 SHA-256 散列

- [ ] sha384 - 计算字符串的 SHA-384 散列

- [ ] sha512 - 计算字符串的 SHA-512 散列

  

## hash - 计算字符串 哈希 值

支持SHA1, SHA224, SHA256, SHA384 和 SHA512，MD5

```python
def hash(cls, text: Union[str, bytes], hash_name: str = 'sha1', encoding: str = 'utf-8') -> str:
```

### - 参数说明

| 参数      | 类型       | 必选 | 默认值 | 说明                              |
| --------- | ---------- | ---- | ------ | --------------------------------- |
| text      | str\|bytes | Y    | 无     | 需要进行 hash 计算的 字符串或字节 |
| hash_name | str        | Y    | -1     | 指定哈希算法                      |
| encoding  | str        | N    | utf-8  | 指定字符串编码，默认utf-8         |

##### - hash_name可选

* MD5
* SHA1
* SHA224
* SHA256
* SHA384
* SHA512

### - 使用示例

```python
# MD5
Hash.md5('123456')
Hash.md5('中文')

# SHA
Hash.sha1('123456')
Hash.sha224('123456')
Hash.sha256('123456')
Hash.sha384('123456')
Hash.sha512('123456')
```



## fileHash - 计算文件 哈希 值

计算文件的哈希值，文件过大时可分块读取。

### - 参数说明

| 参数       | 类型 | 必选 | 默认值 | 说明                      |
| ---------- | ---- | ---- | ------ | ------------------------- |
| fpath      | str  | Y    | 无     | 文件路径                  |
| hash_name  | str  | Y    | -1     | 指定哈希算法，默认为SHA-1 |
| chunk_size | int  | N    | 无     | 分块读取文件              |

##### - hash_name可选

* MD5
* SHA1
* SHA224
* SHA256
* SHA384
* SHA512

### - 使用示例



## Hash实例使用

可创建Hash实例对象，对bytes数据进行哈希计算。

```python
# 实例对象
def __init__(self, hash_name: str, encoding: str = 'utf-8'):
    pass

# 添加数据
def update(self, data: Union[str, bytes]):
	pass    

# 返回哈希值
def hexdigest(self) -> str:
    pass
```

### - 使用示例

```python
# 计算 md5 散列值
Hash(Hash.MD5).update("123456").hexdigest()

# 计算 SHA-1 散列值
sha1Hash = Hash(Hash.SHA1).update("123456").update("abcd").hexdigest()
```



