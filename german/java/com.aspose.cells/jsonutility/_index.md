---
title: "JsonUtility"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Hilfsklasse zur Verarbeitung von JSON dar."
type: docs
url: /de/java/com.aspose.cells/jsonutility/
---

**Inheritance:**
java.lang.Object
```
public class JsonUtility
```

Stellt die Hilfsklasse zur Verarbeitung von JSON dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [JsonUtility()](#JsonUtility--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportRangeToJson(Range range, ExportRangeToJsonOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-) | Exportiere den Bereich in eine JSON-Datei. |
| [exportRangeToJson(Range range, JsonSaveOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-) | Exportiere den Bereich in eine JSON-Datei. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)](#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-) | Importiere die JSON-Zeichenkette. |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportRangeToJson(Range range, ExportRangeToJsonOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-}
```
public static String exportRangeToJson(Range range, ExportRangeToJsonOptions options)
```


Exportiere den Bereich in eine JSON-Datei.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode ExportRangeToJson(Range range, JsonSaveOptions options). Diese Eigenschaft wird 6 Monate nach November 2022 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Der Bereich. |
| options | [ExportRangeToJsonOptions](../../com.aspose.cells/exportrangetojsonoptions) | Die Optionen für den Export. |

**Returns:**
java.lang.String - Der JSON-String-Wert.
### exportRangeToJson(Range range, JsonSaveOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-}
```
public static String exportRangeToJson(Range range, JsonSaveOptions options)
```


Exportiere den Bereich in eine JSON-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Der Bereich. |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Die Optionen für den Export. |

**Returns:**
java.lang.String - Der JSON-String-Wert.
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


Importiere die JSON-Zeichenkette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| JSON | java.lang.String | Der JSON-String. |
| cells | [Cells](../../com.aspose.cells/cells) | Die Zellen. |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |
| option | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) | Die Optionen für das Importieren des JSON-Strings. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

