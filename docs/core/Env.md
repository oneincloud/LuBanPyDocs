# Env - 环境变量管理器

`Env`环境变量提供程序运行状态的信息和简单的值共享。



## 一、环境常量

### 1.1、应用运行时常量

| 常量                      | 只读 | 类型 | 描术                                                         |
| ------------------------- | ---- | ---- | ------------------------------------------------------------ |
| `__BOOT_AT__`             | Y    | int  | 获取应用启动时间截                                           |
| `__IS_FROZEN__`           | Y    | bool | 应用是否已打包，当前已支持工具：PyInstaller                  |
| `__PROCESS_ID__`          | Y    | int  | 获取当前进程ID                                               |
| `__PROCESS_NAME__`        | Y    | str  | 获取当前进程名称                                             |
| `__PARENT_PROCESS_ID__`   | Y    | int  | 获取父进程ID                                                 |
| `__PARENT_PROCESS_NAME__` | Y    | str  | 获取父进程名称                                               |
| `__BOOT_PROCESS_ID__`     | Y    | int  | 获取应用入口进程ID                                           |
| `__TOP_PROCESS_ID__`      | Y    | int  | 获取主进程ID                                                 |
| `__IS_TOP_PROCESS__`      | Y    | bool | 检查当前进程是否主进程                                       |
| `__RUNTIME_MODE__`        | Y    | int  | 获取应用运行模式代码<br />0 - 正常模式（单进程模式）<br />1 - 应用模式（支持多进程） |



### 1.2、应用目录常量

| 目录         | 只读 | 描述                                                         |
| ------------ | ---- | ------------------------------------------------------------ |
| ROOT_PATH    | N    | [系统]项目根目录，打包后为exe当前执行目录，只能在非打包模式进修ROOT_PATH |
| SOURCE_PATH  | Y    | [系统]源代码根目录，打包后为解包临时目录                     |
| HOME_PATH    | Y    | [系统]系统用户目录                                           |
| CONFIG_PATH  | Y    | 系统配置文件目录，建议与项目编译打包发布，可通过.env配置覆盖 |
| RUNTIME_PATH | Y    | 运行时目录（缓存、临时文件、日志）                           |
| DATA_PATH    | Y    | 数据目录，一般存放数据库文件，例如sqlite，默认`runtime/data`目录 |
| STORAGE_PATH | Y    | 存储目录，一般是图片存放，默认`runtime/storage`目录          |
| CACHE_PATH   | Y    | 缓存目录，默认`runtime/cache`目录                            |
| LOG_PATH     | Y    | 日志目录，默认`runtime/log`目录                              |
| TMP_PATH     | Y    | 临时目录，默认`runtime/tmp`目录                              |



### 1.3、应用信息常量

| 常量         | 只读 | 类型 | 描术                                                     |
| ------------ | ---- | ---- | -------------------------------------------------------- |
| DEBUG        | N    | bool | 是否开启调试模式，设置为TRUE强制开启调式模式，支持setter |
| PRODUCTION   | Y    | bool | 是否生产环境                                             |
| PROJECT_NAME | N    | str  | 项目名称，英文，合法的文件名称                           |
| APP_NAME     | N    | str  | 应用名称，用于显示的名称，未设置时与PROJECT_NAME相同     |
| VERSION      | N    | str  | 应用版本号                                               |



## 二、Env组件方法清单

### set

### get

### pop

### remove

### clear



