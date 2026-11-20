---
title: "GridJsLogger"
second_title: "Справочник API Aspose.Cells for Java"
description: "Предоставляет легковесную систему журналирования для сервера GridJs."
type: docs
url: /ru/java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

Предоставляет легковесную систему логирования для сервера GridJs. Поддерживает вывод в консоль и файл с настраиваемыми уровнями журналирования. Уровень по умолчанию — None. В сборке DEBUG уровень по умолчанию — Debug (выводит все сообщения). Поддерживает ротацию файлов журнала по дню/неделе/месяцу.
## Методы

| Метод | Описание |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | Закрывает запись в файл журнала и отключает вывод в файл. |
| [debug(String message)](#debug-java.lang.String-) | Записывает сообщение уровня debug. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | Записывает сообщение уровня error. |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | Возвращает, выводятся ли сообщения журнала в консоль. |
| [getEnableFileOutput()](#getEnableFileOutput--) | Возвращает, выводятся ли сообщения журнала в файл. |
| [getLevel()](#getLevel--) | Возвращает минимальный уровень журнала. |
| [getLogFilePath()](#getLogFilePath--) | Возвращает текущий путь к файлу журнала или null, если не установлен. |
| [getMaxFileSize()](#getMaxFileSize--) | Возвращает максимальный размер (в байтах) одного файла журнала до ротации. |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | Записывает сообщение уровня info. |
| [log(int level, String message)](#log-int-java.lang.String-) | Записывает сообщение на указанном уровне. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | Устанавливает, выводить ли сообщения журнала в консоль. |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | Устанавливает, выводить ли сообщения журнала в файл. |
| [setLevel(int value)](#setLevel-int-) | Устанавливает минимальный уровень журнала. |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | Устанавливает каталог журнала со стратегией ежедневного ротации файлов и включает вывод в файл. |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | Устанавливает каталог журнала со стратегией ротации файлов и включает вывод в файл. |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | Устанавливает каталог журнала со стратегией ротации файлов и включает вывод в файл. |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | Устанавливает путь к файлу журнала и включает вывод в файл (режим одного файла, без ротации). |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | Устанавливает путь к файлу журнала и включает вывод в файл (режим одного файла, без ротации). |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | Устанавливает максимальный размер (в байтах) одного файла журнала перед ротацией. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | Записывает сообщение уровня предупреждения. |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


Закрывает запись в файл журнала и отключает вывод в файл.

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


Записывает сообщение уровня debug.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| сообщение | java.lang.String |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


Записывает сообщение уровня error.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| сообщение | java.lang.String |  |

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


Получает, выводятся ли сообщения журнала в консоль. По умолчанию false.

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


Получает, выводятся ли сообщения журнала в файл. По умолчанию false. Необходимо вызвать [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) или [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) перед включением.

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


Получает минимальный уровень журнала. Сообщения ниже этого уровня будут игнорироваться. По умолчанию None.

Смотрите [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


Возвращает текущий путь к файлу журнала или null, если не установлен.

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


Получает максимальный размер (в байтах) одного файла журнала перед ротацией. Действует только при включённой ротации. 0 означает отсутствие ограничения размера. По умолчанию 0.

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


Записывает сообщение уровня info.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| сообщение | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


Записывает сообщение на указанном уровне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel). Уровень журнала. |
| сообщение | java.lang.String | Сообщение для записи. |

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


Устанавливает, выводить ли сообщения журнала в консоль. По умолчанию false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


Устанавливает, выводить ли сообщения журнала в файл. По умолчанию false. Необходимо вызвать [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) или [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) перед включением.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


Устанавливает минимальный уровень журнала. Сообщения ниже этого уровня будут игнорироваться. По умолчанию None.

Смотрите [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


Устанавливает каталог журнала со стратегией ежедневной ротации файлов и включает вывод в файл. Файлы журнала будут называться так: gridjs\_\{period\}.log

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| каталог | java.lang.String | Каталог для хранения файлов журнала. |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


Устанавливает каталог журнала со стратегией ротации файлов и включает вывод в файл. Файлы журнала будут называться так: gridjs\_\{period\}.log

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| каталог | java.lang.String | Каталог для хранения файлов журнала. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). Стратегия ротации (Daily/Weekly/Monthly). |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


Устанавливает каталог журнала со стратегией ротации файлов и включает вывод в файл. Файлы журнала будут называться так: \{prefix\}\_\{period\}.log Примеры: gridjs\_2026-07-27.log (Daily), gridjs\_2026-W30.log (Weekly), gridjs\_2026-07.log (Monthly)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| каталог | java.lang.String | Каталог для хранения файлов журнала. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). Стратегия ротации (Daily/Weekly/Monthly). |
| filePrefix | java.lang.String | Префикс имени файла. |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


Устанавливает путь к файлу журнала и включает вывод в файл (режим одного файла, без ротации). Добавляет к существующему файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Полный путь к файлу журнала. |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


Устанавливает путь к файлу журнала и включает вывод в файл (режим одного файла, без ротации).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Полный путь к файлу журнала. |
| добавить | boolean | Определяет, добавлять ли к существующему файлу. |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


Устанавливает максимальный размер (в байтах) одного файла журнала перед ротацией. Действует только при включённой ротации. 0 означает отсутствие ограничения размера. По умолчанию 0.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | long |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


Записывает сообщение уровня предупреждения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| сообщение | java.lang.String |  |

