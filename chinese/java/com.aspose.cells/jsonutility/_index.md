---
title: "JsonUtility"
second_title: "Aspose.Cells for Java API 参考"
description: "表示处理 json 的实用类。"
type: docs
url: /zh/java/com.aspose.cells/jsonutility/
---

**Inheritance:**
java.lang.Object
```
public class JsonUtility
```

表示处理 json 的实用类。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [JsonUtility()](#JsonUtility--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportRangeToJson(Range range, ExportRangeToJsonOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-) | 将范围导出到 json 文件。 |
| [exportRangeToJson(Range range, JsonSaveOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-) | 将范围导出到 json 文件。 |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)](#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-) | 导入 json 字符串。 |
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportRangeToJson(Range range, ExportRangeToJsonOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-}
```
public static String exportRangeToJson(Range range, ExportRangeToJsonOptions options)
```


将范围导出到 json 文件。

**Remarks**

注意：此成员现已过时。请改用 ExportRangeToJson(Range range, JsonSaveOptions options) 方法。此属性将在自 2022 年 11 月起的 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 范围。 |
| options | [ExportRangeToJsonOptions](../../com.aspose.cells/exportrangetojsonoptions) | 导出选项。 |

**Returns:**
java.lang.String - json 字符串值。
### exportRangeToJson(Range range, JsonSaveOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-}
```
public static String exportRangeToJson(Range range, JsonSaveOptions options)
```


将范围导出到 json 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 范围。 |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | 导出选项。 |

**Returns:**
java.lang.String - json 字符串值。
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


导入 json 字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| json | java.lang.String | json 字符串。 |
| cells | [Cells](../../com.aspose.cells/cells) | Cells。 |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |
| option | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) | 导入 JSON 字符串的选项。 |

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

