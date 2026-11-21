---
title: "JsonUtility"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la clase de utilidad para procesar JSON."
type: docs
url: /es/java/com.aspose.cells/jsonutility/
---

**Inheritance:**
java.lang.Object
```
public class JsonUtility
```

Representa la clase de utilidad para procesar JSON.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [JsonUtility()](#JsonUtility--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportRangeToJson(Range range, ExportRangeToJsonOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-) | Exportando el rango a un archivo json. |
| [exportRangeToJson(Range range, JsonSaveOptions options)](#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-) | Exportando el rango a un archivo json. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [importData(String json, Cells cells, int row, int column, JsonLayoutOptions option)](#importData-java.lang.String-com.aspose.cells.Cells-int-int-com.aspose.cells.JsonLayoutOptions-) | Importar la cadena json. |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportRangeToJson(Range range, ExportRangeToJsonOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.ExportRangeToJsonOptions-}
```
public static String exportRangeToJson(Range range, ExportRangeToJsonOptions options)
```


Exportando el rango a un archivo json.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método ExportRangeToJson(Range range, JsonSaveOptions options). Esta propiedad será eliminada 6 meses después desde noviembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | El rango. |
| options | [ExportRangeToJsonOptions](../../com.aspose.cells/exportrangetojsonoptions) | Las opciones de exportación. |

**Returns:**
java.lang.String - El valor de la cadena json.
### exportRangeToJson(Range range, JsonSaveOptions options) {#exportRangeToJson-com.aspose.cells.Range-com.aspose.cells.JsonSaveOptions-}
```
public static String exportRangeToJson(Range range, JsonSaveOptions options)
```


Exportando el rango a un archivo json.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | El rango. |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Las opciones de exportación. |

**Returns:**
java.lang.String - El valor de la cadena json.
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


Importar la cadena json.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| json | java.lang.String | La cadena json. |
| cells | [Cells](../../com.aspose.cells/cells) | Las Celdas. |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |
| option | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) | Las opciones de importación de la cadena json. |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

