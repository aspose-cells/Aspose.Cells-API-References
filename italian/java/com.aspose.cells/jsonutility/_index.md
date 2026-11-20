---
title: "JsonUtility"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la classe di utilità per l'elaborazione del JSON."
type: docs
url: /it/java/com.aspose.cells/jsonutility/
---

**Inheritance:**
java.lang.Object
```
public class JsonUtility
```

Rappresenta la classe di utilità per l'elaborazione del JSON.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [JsonUtility()](#JsonUtility--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportRangeToJson(Range range, ExportRangeToJsonOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-) | Esportazione dell'intervallo in un file json. |
| [exportRangeToJson(Range range, JsonSaveOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-) | Esportazione dell'intervallo in un file json. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)](#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-) | Importa la stringa json. |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportRangeToJson(Range range, ExportRangeToJsonOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-}
```
public static String exportRangeToJson(Range range, ExportRangeToJsonOptions options)
```


Esportazione dell'intervallo in un file json.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo ExportRangeToJson(Range range, JsonSaveOptions options). Questa proprietà verrà rimossa tra 6 mesi a partire da novembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | L'intervallo. |
| options | [ExportRangeToJsonOptions](../../com.aspose.cells/exportrangetojsonoptions) | Le opzioni di esportazione. |

**Returns:**
java.lang.String - Il valore della stringa json.
### exportRangeToJson(Range range, JsonSaveOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-}
```
public static String exportRangeToJson(Range range, JsonSaveOptions options)
```


Esportazione dell'intervallo in un file json.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | L'intervallo. |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Le opzioni di esportazione. |

**Returns:**
java.lang.String - Il valore della stringa json.
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


Importa la stringa json.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| json | java.lang.String | La stringa json. |
| cells | [Cells](../../com.aspose.cells/cells) | Le Cells. |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |
| option | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) | Le opzioni di importazione della stringa json. |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

