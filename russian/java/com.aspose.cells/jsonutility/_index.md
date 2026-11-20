---
title: "JsonUtility"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет вспомогательный класс обработки json."
type: docs
url: /ru/java/com.aspose.cells/jsonutility/
---

**Inheritance:**
java.lang.Object
```
public class JsonUtility
```

Представляет вспомогательный класс обработки json.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [JsonUtility()](#JsonUtility--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportRangeToJson(Range range, ExportRangeToJsonOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-) | Экспорт диапазона в json‑файл. |
| [exportRangeToJson(Range range, JsonSaveOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-) | Экспорт диапазона в json‑файл. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)](#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-) | Импортировать json‑строку. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonUtility() {#JsonUtility--}
```
public JsonUtility()
```


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
### exportRangeToJson(Range range, ExportRangeToJsonOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-}
```
public static String exportRangeToJson(Range range, ExportRangeToJsonOptions options)
```


Экспорт диапазона в json‑файл.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод ExportRangeToJson(Range range, JsonSaveOptions options). Это свойство будет удалено через 6 месяцев, начиная с ноября 2022 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Диапазон. |
| options | [ExportRangeToJsonOptions](../../com.aspose.cells/exportrangetojsonoptions) | Параметры экспорта. |

**Returns:**
java.lang.String — значение json‑строки.
### exportRangeToJson(Range range, JsonSaveOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-}
```
public static String exportRangeToJson(Range range, JsonSaveOptions options)
```


Экспорт диапазона в json‑файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Диапазон. |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Параметры экспорта. |

**Returns:**
java.lang.String — значение json‑строки.
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
### importData(String json, Cells cells, int row, int column, JsonLayoutOptions option) {#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-}
```
public static int[] importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)
```


Импортировать json‑строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| json | java.lang.String | json‑строка. |
| cells | [Cells](../../com.aspose.cells/cells) | Коллекция Cells. |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |
| option | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) | Параметры импорта json‑строки. |

**Returns:**
int[] -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

