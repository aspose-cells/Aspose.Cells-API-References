---
title: "JsonUtility"
second_title: "Aspose.Cells for Java API Referansı"
description: "JSON işleme yardımcı sınıfını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/jsonutility/
---

**Inheritance:**
java.lang.Object
```
public class JsonUtility
```

JSON işleme yardımcı sınıfını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [JsonUtility()](#JsonUtility--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportRangeToJson(Range range, ExportRangeToJsonOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-) | Aralığı json dosyasına dışa aktarıyor. |
| [exportRangeToJson(Range range, JsonSaveOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-) | Aralığı json dosyasına dışa aktarıyor. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)](#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-) | Json dizesini içe aktar. |
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportRangeToJson(Range range, ExportRangeToJsonOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-}
```
public static String exportRangeToJson(Range range, ExportRangeToJsonOptions options)
```


Aralığı json dosyasına dışa aktarıyor.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ExportRangeToJson(Range range, JsonSaveOptions options) yöntemini kullanın. Bu özellik Kasım 2022'den itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Aralık. |
| options | [ExportRangeToJsonOptions](../../com.aspose.cells/exportrangetojsonoptions) | Dışa aktarma seçenekleri. |

**Returns:**
java.lang.String - Json dize değeri.
### exportRangeToJson(Range range, JsonSaveOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-}
```
public static String exportRangeToJson(Range range, JsonSaveOptions options)
```


Aralığı json dosyasına dışa aktarıyor.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Aralık. |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Dışa aktarma seçenekleri. |

**Returns:**
java.lang.String - Json dize değeri.
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


Json dizesini içe aktar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| json | java.lang.String | Json dizesi. |
| cells | [Cells](../../com.aspose.cells/cells) | Hücreler. |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |
| option | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) | Json dizesini içe aktarma seçenekleri. |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

