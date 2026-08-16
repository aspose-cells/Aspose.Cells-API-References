---
title: GridJsLogger
second_title: Aspose.Cells for Java API Reference
description: Provides a lightweight logging system for GridJs server.
type: docs
url: /java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

Provides a lightweight logging system for GridJs server. Supports console and file output with configurable log levels. Default level is None. In DEBUG build, the default level is Debug (outputs all messages). Supports log file rolling by day/week/month.
## Methods

| Method | Description |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | Closes the log file writer and disables file output. |
| [debug(String message)](#debug-java.lang.String-) | Logs a debug level message. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | Logs an error level message. |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | Gets whether to output log messages to the console. |
| [getEnableFileOutput()](#getEnableFileOutput--) | Gets whether to output log messages to a file. |
| [getLevel()](#getLevel--) | Gets the minimum log level. |
| [getLogFilePath()](#getLogFilePath--) | Gets the current log file path, or null if not set. |
| [getMaxFileSize()](#getMaxFileSize--) | Gets the maximum size (in bytes) for a single log file before rolling. |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | Logs an info level message. |
| [log(int level, String message)](#log-int-java.lang.String-) | Logs a message at the specified level. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | Sets whether to output log messages to the console. |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | Sets whether to output log messages to a file. |
| [setLevel(int value)](#setLevel-int-) | Sets the minimum log level. |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | Sets the log directory with daily rolling file strategy and enables file output. |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | Sets the log directory with rolling file strategy and enables file output. |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | Sets the log directory with rolling file strategy and enables file output. |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | Sets the log file path and enables file output (single file mode, no rolling). |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | Sets the log file path and enables file output (single file mode, no rolling). |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | Sets the maximum size (in bytes) for a single log file before rolling. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | Logs a warning level message. |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


Closes the log file writer and disables file output.

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


Logs a debug level message.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


Logs an error level message.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String |  |

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


Gets whether to output log messages to the console. Default is false.

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


Gets whether to output log messages to a file. Default is false. Must call [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) or [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) before enabling.

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


Gets the minimum log level. Messages below this level will be ignored. Default is None.

See [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


Gets the current log file path, or null if not set.

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


Gets the maximum size (in bytes) for a single log file before rolling. Only effective when rolling is enabled. 0 means no size limit. Default is 0.

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


Logs an info level message.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


Logs a message at the specified level.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel). The log level. |
| message | java.lang.String | The message to log. |

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


Sets whether to output log messages to the console. Default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


Sets whether to output log messages to a file. Default is false. Must call [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) or [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) before enabling.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


Sets the minimum log level. Messages below this level will be ignored. Default is None.

See [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


Sets the log directory with daily rolling file strategy and enables file output. Log files will be named as: gridjs\_\{period\}.log

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.lang.String | The directory to store log files. |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


Sets the log directory with rolling file strategy and enables file output. Log files will be named as: gridjs\_\{period\}.log

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.lang.String | The directory to store log files. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). The rolling strategy (Daily/Weekly/Monthly). |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


Sets the log directory with rolling file strategy and enables file output. Log files will be named as: \{prefix\}\_\{period\}.log Examples: gridjs\_2026-07-27.log (Daily), gridjs\_2026-W30.log (Weekly), gridjs\_2026-07.log (Monthly)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.lang.String | The directory to store log files. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). The rolling strategy (Daily/Weekly/Monthly). |
| filePrefix | java.lang.String | The file name prefix. |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


Sets the log file path and enables file output (single file mode, no rolling). Appends to existing file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The full path to the log file. |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


Sets the log file path and enables file output (single file mode, no rolling).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The full path to the log file. |
| append | boolean | Whether to append to existing file. |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


Sets the maximum size (in bytes) for a single log file before rolling. Only effective when rolling is enabled. 0 means no size limit. Default is 0.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | long |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


Logs a warning level message.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String |  |

