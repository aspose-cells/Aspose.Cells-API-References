---
title: "GridPivotTable"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un informe de tabla dinámica en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.gridweb/gridpivottable/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```

Representa un informe de tabla dinámica en una hoja de cálculo. El objeto PivotTable es un miembro de la colección [GridPivotTable](../../com.aspose.gridweb/gridpivottable). La colección PivotTables contiene todos los objetos PivotTable en un control.
## Métodos

| Método | Descripción |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Agrega el campo al área específica. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Agrega el campo al área específica. |
| [calculateData()](#calculateData--) | Calcula los datos de la tabla dinámica en las celdas. |
| [clearAllFields()](#clearAllFields--) | Borra todos los campos de la tabla dinámica. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | Obtiene los campos específicos por el tipo de campo. |
| [fields(String fieldName)](#fields-java.lang.String-) | Obtiene el campo específico por el nombre del campo. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | Actualiza los datos y la configuración de la tabla dinámica desde su fuente de datos. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Agrega el campo al área específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). El tipo de área de campos. |
| baseFieldIndex | int | El índice de campo en los campos base. |

**Returns:**
int - La posición del campo en los campos específicos.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Agrega el campo al área específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). El tipo de área de campos. |
| fieldName | java.lang.String | El nombre en los campos base. |

**Returns:**
int - La posición del campo en los campos específicos. Si no existe un campo con ese nombre, devolver -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Calcula los datos de la tabla dinámica en las celdas.

**Remarks**

Cell.Value en el rango de tabla dinámica podría no devolver el resultado correcto si no se ha llamado al método. Este método calcula los datos con una caché interna de tabla dinámica, no con la fuente de datos original. Por lo tanto, si la fuente de datos cambia, por favor llame primero al método RefreshData().

### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```


Borra todos los campos de la tabla dinámica.

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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```


Obtiene los campos específicos por el tipo de campo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). el tipo de campo. |

**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```


Obtiene el campo específico por el nombre del campo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldName | java.lang.String | el nombre del campo. |

**Returns:**
[GridPivotField](../../com.aspose.gridweb/gridpivotfield) - the specific field
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




### refreshData() {#refreshData--}
```
public void refreshData()
```


Actualiza los datos y la configuración de la tabla dinámica desde su fuente de datos.

**Remarks**

Recopilaremos datos de la fuente de datos a una caché de tabla dinámica, luego calcularemos los datos en la caché en las celdas. Este método solo se usa para recopilar todos los datos en una caché de tabla dinámica.

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

