---
title: "GridJsLogger"
second_title: "Aspose.Cells for Java API 参考"
description: "为 GridJs 服务器提供轻量级日志系统。"
type: docs
url: /zh/java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

为 GridJs 服务器提供轻量级日志系统。支持带可配置日志级别的控制台和文件输出。默认级别为 None。在 DEBUG 构建中，默认级别为 Debug（输出所有消息）。支持按天/周/月滚动日志文件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | 关闭日志文件写入器并禁用文件输出。 |
| [debug(String message)](#debug-java.lang.String-) | 记录调试级别的消息。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | 记录错误级别的消息。 |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | 获取是否将日志消息输出到控制台。 |
| [getEnableFileOutput()](#getEnableFileOutput--) | 获取是否将日志消息输出到文件。 |
| [getLevel()](#getLevel--) | 获取最小日志级别。 |
| [getLogFilePath()](#getLogFilePath--) | 获取当前日志文件路径，如果未设置则为 null。 |
| [getMaxFileSize()](#getMaxFileSize--) | 获取单个日志文件在滚动前的最大大小（字节）。 |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | 记录信息级别的消息。 |
| [log(int level, String message)](#log-int-java.lang.String-) | 记录指定级别的消息。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | 设置是否将日志消息输出到控制台。 |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | 设置是否将日志消息输出到文件。 |
| [setLevel(int value)](#setLevel-int-) | 设置最小日志级别。 |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | 设置日志目录，使用每日滚动文件策略并启用文件输出。 |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | 设置日志目录，使用滚动文件策略并启用文件输出。 |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | 设置日志目录，使用滚动文件策略并启用文件输出。 |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | 设置日志文件路径并启用文件输出（单文件模式，不滚动）。 |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | 设置日志文件路径并启用文件输出（单文件模式，不滚动）。 |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | 设置单个日志文件在滚动前的最大大小（字节）。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | 记录警告级别的消息。 |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


关闭日志文件写入器并禁用文件输出。

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


记录调试级别的消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 消息 | java.lang.String |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


记录错误级别的消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 消息 | java.lang.String |  |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableConsoleOutput() {#getEnableConsoleOutput--}
```
public static boolean getEnableConsoleOutput()
```


获取是否将日志消息输出到控制台。默认值为 false。

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


获取是否将日志消息输出到文件。默认值为 false。必须在启用之前调用 [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\\#setLogFile-String-) 或 [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\\#setLogDirectory-String-)。

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


获取最低日志级别。低于此级别的消息将被忽略。默认值为 None。

参见 [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel)。

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


获取当前日志文件路径，如果未设置则为 null。

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


获取单个日志文件在滚动前的最大大小（字节）。仅在启用滚动时生效。0 表示无限制大小。默认值为 0。

**Returns:**
long
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### info(String message) {#info-java.lang.String-}
```
public static void info(String message)
```


记录信息级别的消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 消息 | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


记录指定级别的消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel)。日志级别。 |
| 消息 | java.lang.String | 要记录的消息。 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setEnableConsoleOutput(boolean value) {#setEnableConsoleOutput-boolean-}
```
public static void setEnableConsoleOutput(boolean value)
```


设置是否将日志消息输出到控制台。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


设置是否将日志消息输出到文件。默认值为 false。必须在启用之前调用 [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\\#setLogFile-String-) 或 [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\\#setLogDirectory-String-)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


设置最低日志级别。低于此级别的消息将被忽略。默认值为 None。

参见 [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


设置日志目录并使用每日滚动文件策略，同时启用文件输出。日志文件将命名为：gridjs\\_\\{period\\}.log

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目录 | java.lang.String | 用于存放日志文件的目录。 |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


设置日志目录并使用滚动文件策略，同时启用文件输出。日志文件将命名为：gridjs\\_\\{period\\}.log

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目录 | java.lang.String | 用于存放日志文件的目录。 |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling)。滚动策略（每日/每周/每月）。 |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


设置日志目录并使用滚动文件策略，同时启用文件输出。日志文件将命名为：\\{prefix\\}\\_\\{period\\}.log 示例：gridjs\\_2026-07-27.log（每日），gridjs\\_2026-W30.log（每周），gridjs\\_2026-07.log（每月）

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目录 | java.lang.String | 用于存放日志文件的目录。 |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling)。滚动策略（每日/每周/每月）。 |
| filePrefix | java.lang.String | 文件名前缀。 |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


设置日志文件路径并启用文件输出（单文件模式，无滚动）。追加到已有文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 日志文件的完整路径。 |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


设置日志文件路径并启用文件输出（单文件模式，不滚动）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 日志文件的完整路径。 |
| 追加 | boolean | 是否追加到已有文件。 |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


设置单个日志文件在滚动前的最大大小（字节）。仅在启用滚动时生效。0 表示无限制大小。默认值为 0。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | long |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


记录警告级别的消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 消息 | java.lang.String |  |

