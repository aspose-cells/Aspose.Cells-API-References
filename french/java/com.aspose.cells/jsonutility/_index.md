---
title: "JsonUtility"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la classe utilitaire de traitement du JSON."
type: docs
url: /fr/java/com.aspose.cells/jsonutility/
---

**Inheritance:**
java.lang.Object
```
public class JsonUtility
```

Représente la classe utilitaire de traitement du JSON.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [JsonUtility()](#JsonUtility--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportRangeToJson(Range range, ExportRangeToJsonOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-) | Exportation de la plage vers un fichier json. |
| [exportRangeToJson(Range range, JsonSaveOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-) | Exportation de la plage vers un fichier json. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)](#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-) | Importer la chaîne json. |
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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportRangeToJson(Range range, ExportRangeToJsonOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-}
```
public static String exportRangeToJson(Range range, ExportRangeToJsonOptions options)
```


Exportation de la plage vers un fichier json.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode ExportRangeToJson(Range range, JsonSaveOptions options). Cette propriété sera supprimée dans 6 mois à compter de novembre 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | La plage. |
| options | [ExportRangeToJsonOptions](../../com.aspose.cells/exportrangetojsonoptions) | Les options d'exportation. |

**Returns:**
java.lang.String - La valeur de la chaîne json.
### exportRangeToJson(Range range, JsonSaveOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-}
```
public static String exportRangeToJson(Range range, JsonSaveOptions options)
```


Exportation de la plage vers un fichier json.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | La plage. |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Les options d'exportation. |

**Returns:**
java.lang.String - La valeur de la chaîne json.
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


Importer la chaîne json.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| json | java.lang.String | La chaîne json. |
| cells | [Cells](../../com.aspose.cells/cells) | Les Cells. |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |
| option | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) | Les options d'importation de la chaîne json. |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

