---
title: "SpreadsheetSplitter"
second_title: "Справочник API Aspose.Cells for Java"
description: "Разделяет файл таблицы на несколько частей."
type: docs
url: /ru/java/com.aspose.cells/spreadsheetsplitter/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetSplitter
```

Разделяет файл таблицы на несколько частей.

**Example**

```
         SpreadsheetSplitter.process("template.xlsx", "split.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeSplitOptions options)](#process-com.aspose.cells.LowCodeSplitOptions-) | Разделяет файл таблицы на несколько частей. |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Разделяет указанный шаблонный файл на несколько частей. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### process(LowCodeSplitOptions options) {#process-com.aspose.cells.LowCodeSplitOptions-}
```
public static void process(LowCodeSplitOptions options)
```


Разделяет файл таблицы на несколько частей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [LowCodeSplitOptions](../../com.aspose.cells/lowcodesplitoptions) | Параметры разделения электронной таблицы. |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Разделяет указанный шаблонный файл на несколько частей.

**Remarks**

Файлы вывода будут создаваться из указанного результирующего файла путем добавления порядкового номера листа и части разделения. Например, если указанный файл вывода — Split.xlsx, то сгенерированные файлы будут Split\_0\_0.xlsx, Split\_0\_1.xlsx, ..., Split\_1\_0.xlsx, ...

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFile | java.lang.String | Шаблонный файл для разделения. |
| resultFile | java.lang.String | Результирующий файл (шаблон имени). |

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

