---
title: "JsonUtility"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل فئة الأدوات لمعالجة json."
type: docs
url: /ar/java/com.aspose.cells/jsonutility/
---

**Inheritance:**
java.lang.Object
```
public class JsonUtility
```

يمثل فئة الأدوات لمعالجة json.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [JsonUtility()](#JsonUtility--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportRangeToJson(Range range, ExportRangeToJsonOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-) | تصدير النطاق إلى ملف json. |
| [exportRangeToJson(Range range, JsonSaveOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-) | تصدير النطاق إلى ملف json. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)](#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-) | استيراد سلسلة json. |
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportRangeToJson(Range range, ExportRangeToJsonOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-}
```
public static String exportRangeToJson(Range range, ExportRangeToJsonOptions options)
```


تصدير النطاق إلى ملف json.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام طريقة ExportRangeToJson(Range range, JsonSaveOptions options). سيتم إزالة هذه الخاصية بعد 6 أشهر منذ نوفمبر 2022. تُعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | النطاق. |
| options | [ExportRangeToJsonOptions](../../com.aspose.cells/exportrangetojsonoptions) | خيارات التصدير. |

**Returns:**
java.lang.String - قيمة سلسلة json.
### exportRangeToJson(Range range, JsonSaveOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-}
```
public static String exportRangeToJson(Range range, JsonSaveOptions options)
```


تصدير النطاق إلى ملف json.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | النطاق. |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | خيارات التصدير. |

**Returns:**
java.lang.String - قيمة سلسلة json.
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


استيراد سلسلة json.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| json | java.lang.String | سلسلة json. |
| cells | [Cells](../../com.aspose.cells/cells) | الخلايا. |
| صف | int | The row index. |
| عمود | int | The column index. |
| option | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) | خيارات استيراد سلسلة json. |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

