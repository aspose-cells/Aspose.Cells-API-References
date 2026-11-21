---
title: "JsonUtility"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar verktygsklassen för bearbetning av json."
type: docs
url: /sv/java/com.aspose.cells/jsonutility/
---

**Inheritance:**
java.lang.Object
```
public class JsonUtility
```

Representerar verktygsklassen för bearbetning av json.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [JsonUtility()](#JsonUtility--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportRangeToJson(Range range, ExportRangeToJsonOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-) | Exporterar intervallet till en json-fil. |
| [exportRangeToJson(Range range, JsonSaveOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-) | Exporterar intervallet till en json-fil. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)](#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-) | Importera json-strängen. |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportRangeToJson(Range range, ExportRangeToJsonOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-}
```
public static String exportRangeToJson(Range range, ExportRangeToJsonOptions options)
```


Exporterar intervallet till en json-fil.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället ExportRangeToJson(Range range, JsonSaveOptions options) metoden. Denna egenskap kommer att tas bort 6 månader senare, sedan november 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Intervallet. |
| options | [ExportRangeToJsonOptions](../../com.aspose.cells/exportrangetojsonoptions) | Exportalternativen. |

**Returns:**
java.lang.String - json-strängens värde.
### exportRangeToJson(Range range, JsonSaveOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-}
```
public static String exportRangeToJson(Range range, JsonSaveOptions options)
```


Exporterar intervallet till en json-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Intervallet. |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Exportalternativen. |

**Returns:**
java.lang.String - json-strängens värde.
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


Importera json-strängen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| json | java.lang.String | Json-strängen. |
| cells | [Cells](../../com.aspose.cells/cells) | Cellerna. |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |
| option | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) | Alternativen för att importera json-strängen. |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

