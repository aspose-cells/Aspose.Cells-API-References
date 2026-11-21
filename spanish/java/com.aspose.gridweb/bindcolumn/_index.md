---
title: "BindColumn"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "BindColumn."
type: docs
url: /es/java/com.aspose.gridweb/bindcolumn/
---

**Inheritance:**
java.lang.Object
```
public class BindColumn
```

BindColumn.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [BindColumn()](#BindColumn--) | Constructor predeterminado. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeStyle()](#getAlternativeStyle--) | Obtiene el estilo alternativo de la columna. |
| [getCaption()](#getCaption--) | El título de la columna. |
| [getClass()](#getClass--) |  |
| [getColumnHeaderStyle()](#getColumnHeaderStyle--) | Obtiene el estilo de la columna. |
| [getCommandName()](#getCommandName--) | El nombre del comando de la columna. |
| [getCommandText()](#getCommandText--) | El texto del comando que se muestra de la columna. |
| [getCustomFormat()](#getCustomFormat--) | La cadena de formato personalizada. |
| [getDataField()](#getDataField--) | Obtiene la cadena del nombre del campo de datos. |
| [getEnableSort()](#getEnableSort--) | Indica si el usuario puede hacer clic en el encabezado de la columna para ordenar por este campo. |
| [getImageUrl()](#getImageUrl--) | La URL de la imagen del hipervínculo del comando. |
| [getName()](#getName--) | Solo se usa en tiempo de diseño. |
| [getNumberType()](#getNumberType--) | Obtiene el tipo numérico de la columna. |
| [getStyle()](#getStyle--) | Obtiene el estilo de la columna. |
| [getUseAlternativeStyle()](#getUseAlternativeStyle--) | Obtiene si se debe usar el estilo alternativo para la columna. |
| [getValidation()](#getValidation--) | Obtiene el objeto de validación de la columna. |
| [getWidth()](#getWidth--) | Obtiene o establece el ancho de la columna. Solo se aceptan píxeles o puntos. |
| [hashCode()](#hashCode--) |  |
| [isAutoCreated()](#isAutoCreated--) | Indica si la columna se crea automáticamente. |
| [isReadOnly()](#isReadOnly--) | Indica si la columna es de solo lectura. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlternativeStyle(GridTableItemStyle value)](#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-) | Establece el estilo alternativo de la columna. |
| [setAutoCreated(boolean value)](#setAutoCreated-boolean-) | Indica si la columna se crea automáticamente. |
| [setCaption(String value)](#setCaption-java.lang.String-) | El título de la columna. |
| [setColumnHeaderStyle(GridTableItemStyle value)](#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-) | Establece el estilo de la columna. |
| [setCommandName(String value)](#setCommandName-java.lang.String-) | El nombre del comando de la columna. |
| [setCommandText(String value)](#setCommandText-java.lang.String-) | El texto del comando que se muestra de la columna. |
| [setCustomFormat(String value)](#setCustomFormat-java.lang.String-) | La cadena de formato personalizada. |
| [setDataField(String value)](#setDataField-java.lang.String-) | Establece la cadena del nombre del campo de datos. |
| [setEnableSort(boolean value)](#setEnableSort-boolean-) | Indica si el usuario puede hacer clic en el encabezado de la columna para ordenar por este campo. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | La URL de la imagen del hipervínculo del comando. |
| [setNumberType(int value)](#setNumberType-int-) | Establece el tipo numérico de la columna. |
| [setReadOnly(boolean value)](#setReadOnly-boolean-) | Indica si la columna es de solo lectura. |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Establece el estilo de la columna. |
| [setUseAlternativeStyle(boolean value)](#setUseAlternativeStyle-boolean-) | Establece si se debe usar el estilo alternativo para la columna. |
| [setValidation(GridValidation value)](#setValidation-com.aspose.gridweb.GridValidation-) | Establece el objeto de validación de la columna. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Obtiene o establece el ancho de la columna. Solo se aceptan píxeles o puntos. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BindColumn() {#BindColumn--}
```
public BindColumn()
```


Constructor predeterminado.

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
### getAlternativeStyle() {#getAlternativeStyle--}
```
public GridTableItemStyle getAlternativeStyle()
```


Obtiene el estilo alternativo de la columna.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCaption() {#getCaption--}
```
public String getCaption()
```


El título de la columna.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnHeaderStyle() {#getColumnHeaderStyle--}
```
public GridTableItemStyle getColumnHeaderStyle()
```


Obtiene el estilo de la columna.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCommandName() {#getCommandName--}
```
public String getCommandName()
```


El nombre del comando de la columna. Se creará un Hipervínculo CellCommand en la celda vinculada si se establece la propiedad CommandName.

**Returns:**
java.lang.String
### getCommandText() {#getCommandText--}
```
public String getCommandText()
```


El texto del comando que se muestra de la columna. Si se establece en null, la celda usará el valor del campo como texto del comando.

**Returns:**
java.lang.String
### getCustomFormat() {#getCustomFormat--}
```
public String getCustomFormat()
```


La cadena de formato personalizada.

**Returns:**
java.lang.String
### getDataField() {#getDataField--}
```
public String getDataField()
```


Obtiene la cadena del nombre del campo de datos.

**Returns:**
java.lang.String
### getEnableSort() {#getEnableSort--}
```
public boolean getEnableSort()
```


Indica si el usuario puede hacer clic en el encabezado de la columna para ordenar por este campo.

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


La URL de la imagen del hipervínculo del comando.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Solo se usa en tiempo de diseño.

**Returns:**
java.lang.String
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Obtiene el tipo numérico de la columna.

Ver [NumberType](../../com.aspose.gridweb/numbertype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Obtiene el estilo de la columna.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getUseAlternativeStyle() {#getUseAlternativeStyle--}
```
public boolean getUseAlternativeStyle()
```


Obtiene si se debe usar el estilo alternativo para la columna.

**Returns:**
boolean
### getValidation() {#getValidation--}
```
public GridValidation getValidation()
```


Obtiene el objeto de validación de la columna.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Obtiene o establece el ancho de la columna. Solo se aceptan píxeles o puntos.

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoCreated() {#isAutoCreated--}
```
public boolean isAutoCreated()
```


Indica si la columna se crea automáticamente. Si es verdadero, la columna se eliminará cuando el usuario cambie la fuente de datos en tiempo de diseño.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Indica si la columna es de solo lectura.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAlternativeStyle(GridTableItemStyle value) {#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setAlternativeStyle(GridTableItemStyle value)
```


Establece el estilo alternativo de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoCreated(boolean value) {#setAutoCreated-boolean-}
```
public void setAutoCreated(boolean value)
```


Indica si la columna se crea automáticamente. Si es verdadero, la columna se eliminará cuando el usuario cambie la fuente de datos en tiempo de diseño.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


El título de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setColumnHeaderStyle(GridTableItemStyle value) {#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setColumnHeaderStyle(GridTableItemStyle value)
```


Establece el estilo de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setCommandName(String value) {#setCommandName-java.lang.String-}
```
public void setCommandName(String value)
```


El nombre del comando de la columna. Se creará un Hipervínculo CellCommand en la celda vinculada si se establece la propiedad CommandName.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCommandText(String value) {#setCommandText-java.lang.String-}
```
public void setCommandText(String value)
```


El texto del comando que se muestra de la columna. Si se establece en null, la celda usará el valor del campo como texto del comando.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCustomFormat(String value) {#setCustomFormat-java.lang.String-}
```
public void setCustomFormat(String value)
```


La cadena de formato personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDataField(String value) {#setDataField-java.lang.String-}
```
public void setDataField(String value)
```


Establece la cadena del nombre del campo de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setEnableSort(boolean value) {#setEnableSort-boolean-}
```
public void setEnableSort(boolean value)
```


Indica si el usuario puede hacer clic en el encabezado de la columna para ordenar por este campo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


La URL de la imagen del hipervínculo del comando.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Establece el tipo numérico de la columna.

Ver [NumberType](../../com.aspose.gridweb/numbertype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setReadOnly(boolean value) {#setReadOnly-boolean-}
```
public void setReadOnly(boolean value)
```


Indica si la columna es de solo lectura.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Establece el estilo de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setUseAlternativeStyle(boolean value) {#setUseAlternativeStyle-boolean-}
```
public void setUseAlternativeStyle(boolean value)
```


Establece si se debe usar el estilo alternativo para la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setValidation(GridValidation value) {#setValidation-com.aspose.gridweb.GridValidation-}
```
public void setValidation(GridValidation value)
```


Establece el objeto de validación de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridValidation](../../com.aspose.gridweb/gridvalidation) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Obtiene o establece el ancho de la columna. Solo se aceptan píxeles o puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

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

