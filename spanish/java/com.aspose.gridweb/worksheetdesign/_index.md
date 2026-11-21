---
title: "WorksheetDesign"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Hereda de WebWorksheet."
type: docs
url: /es/java/com.aspose.gridweb/worksheetdesign/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control), [com.aspose.gridweb.WebWorksheet](../../com.aspose.gridweb/webworksheet)
```
public class WorksheetDesign extends WebWorksheet
```

Heredado de WebWorksheet. Usado solo en tiempo de diseño.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [WorksheetDesign()](#WorksheetDesign--) | Constructor predeterminado. |
| [WorksheetDesign(MainWeb mw, GridWorksheet gwk)](#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | el constructor con MainWeb y GridWorksheet |
## Métodos

| Método | Descripción |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Ajusta automáticamente el ancho de la columna. |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | Ajusta automáticamente el ancho de la columna. |
| [cancelNewBindRow()](#cancelNewBindRow--) | Cancela y elimina la fila vinculada recién añadida. |
| [commitNewBindRow()](#commitNewBindRow--) | Confirma la fila vinculada recién añadida y la agrega a la fuente de datos. |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | Copia de otro objeto de hoja de cálculo. |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | Después de establecer una fuente de datos para la hoja de cálculo, llama a este método para generar automáticamente las columnas vinculadas. |
| [createNewBindRow()](#createNewBindRow--) | Crea una nueva fila vinculada y la enlaza a la fuente de datos. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Crea un subtotal en la hoja. |
| [dataBind()](#dataBind--) | Vincula la hoja a la Fuente de datos. |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | Elimina una fila vinculada. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Congela paneles en la celda especificada de la hoja de cálculo. |
| [getBindStartColumn()](#getBindStartColumn--) | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar a la fuente de datos. |
| [getBindStartRow()](#getBindStartRow--) | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar a la fuente de datos. |
| [getBindingSource()](#getBindingSource--) | El objeto de fuente de datos realmente enlazado en tiempo de ejecución. |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | Obtiene el número de filas vinculadas en modo de enlace de datos. |
| [getDataMember()](#getDataMember--) | Obtiene el DataMember de la Fuente de datos multivalor. |
| [getDataSource()](#getDataSource--) | Obtiene la Fuente de datos. |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | En modo de enlace de datos, indica si se deben crear encabezados de columnas vinculadas en la hoja. |
| [getIndex()](#getIndex--) | Obtiene el índice de sí mismo dentro de las hojas de cálculo. |
| [getName()](#getName--) | Obtiene el nombre de la hoja. |
| [getUniqueID()](#getUniqueID--) | Obtiene el UniqueID en el Control |
| [getValidations()](#getValidations--) | Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo. |
| [getVisible()](#getVisible--) | Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Agrupa filas. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Agrupa filas. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | Obtiene si la hoja de cálculo está protegida. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | Hace que todas las celdas sean editables. Este es un atributo extendido. |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Hace que todas las celdas sean de solo lectura. Este es un atributo extendido; tenga en cuenta que este atributo no se puede mantener en la celda real; si desea mantener la protección, por favor use setProtect. |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar a la fuente de datos. |
| [setBindStartRow(int value)](#setBindStartRow-int-) | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar a la fuente de datos. |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | Obtiene el número de filas vinculadas en modo de enlace de datos. |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | Establece el DataMember del DataSource multi‑miembro. |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | Establece el DataSource. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Hace que un rango de celdas sea editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Haga que todas las celdas sean de solo lectura llamando al método SetAllCellsReadonly. |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | En modo de enlace de datos, indica si se deben crear encabezados de columnas vinculadas en la hoja. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la hoja. |
| [setProtected(boolean value)](#setProtected-boolean-) | Establece si la hoja de cálculo está protegida. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Hace que un rango de celdas sea de solo lectura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Primero haga que todas las celdas sean editables llamando al método SetAllCellsEditable. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control. |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | Descongela los paneles en la hoja de cálculo. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Desagrupa filas. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorksheetDesign() {#WorksheetDesign--}
```
public WorksheetDesign()
```


Constructor predeterminado.

### WorksheetDesign(MainWeb mw, GridWorksheet gwk) {#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-}
```
public WorksheetDesign(MainWeb mw, GridWorksheet gwk)
```


el constructor con MainWeb y GridWorksheet

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Ajusta automáticamente el ancho de la columna.

**Remarks**

AutoFitColumn es una función imprecisa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |

### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```


Ajusta automáticamente el ancho de la columna. Este método ajusta automáticamente una columna basándose en el contenido de un rango de celdas dentro de la columna desde startRow hasta endRow. AutoFitColumn es una función imprecisa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | índice de columna, basado en cero |
| startRow | int | índice de fila inicial, basado en cero |
| endRow | int | índice de fila final, basado en cero |

### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```


Cancela y elimina la fila vinculada recién añadida.

**Returns:**
int - El índice de fila. Si no se crea una nueva fila vinculada, devuelve -1.
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```


Confirma la fila vinculada recién añadida y la agrega a la fuente de datos.

**Returns:**
int - El índice de fila de la nueva fila. Si no se crea ninguna fila, devuelve -1.
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```


Copia de otro objeto de hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | La otra hoja. |

### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```


Después de establecer una fuente de datos para la hoja de cálculo, llama a este método para generar automáticamente las columnas vinculadas.

### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```


Crea una nueva fila vinculada y la enlaza a la fuente de datos.

**Returns:**
int - El índice de fila de la nueva fila. Si no se crea ninguna fila, devuelve -1.
### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Crea un subtotal en la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnNameRowIndex | int | El índice de fila de la fila de nombre de columna. |
| dataRows | int | El número de filas de datos. |
| groupByColumnIndex | int | El índice de columna de la columna que se agrupará. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). El tipo de función de subtotal. |
| subtotalColumnIndexList | int[] | Los índices de columna que se subtotalearán. |
| functionLabel | java.lang.String | La etiqueta de la función de subtotal. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | El estilo de la línea de total general. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | El estilo de la línea de subtotal. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). El tipo numérico de las celdas de resultado del subtotal. |
| customString | java.lang.String | La cadena de formato personalizada de las celdas de resultado del subtotal. Puede ser nula. |

### dataBind() {#dataBind--}
```
public void dataBind()
```


Vincula la hoja a la Fuente de datos.

### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```


Elimina una fila vinculada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowNum | int | El índice de fila. |

**Returns:**
int - El índice de fila eliminada. Si no se elimina ninguna fila vinculada, devuelve -1.
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
### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Congela paneles en la celda especificada de la hoja de cálculo.

**Remarks**

El índice de fila y el índice de columna no pueden ser ambos cero. El número de filas y el número de columnas tampoco pueden ser ambos cero.

Los dos primeros parámetros especifican la posición congelada y los dos últimos parámetros especifican el área congelada en el panel superior izquierdo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| columna | int | Índice de columna. |
| freezedRows | int | Número de filas visibles en el panel superior, no más que el índice de fila. |
| freezedColumns | int | Número de columnas visibles en el panel izquierdo, no más que el índice de columna. |

### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```


En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar a la fuente de datos.

**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```


En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar a la fuente de datos.

**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```


El objeto de origen de datos realmente enlazado en tiempo de ejecución. Es un objeto DataView cuando la propiedad DataSource es un objeto DataSet, DataTable o DataView.

**Returns:**
java.lang.Iterable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentBindRows() {#getCurrentBindRows--}
```
public int getCurrentBindRows()
```


Obtiene el número de filas vinculadas en modo de enlace de datos.

**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```


Obtiene el DataMember del DataSource multi‑miembro. Generalmente representa un objeto DataTable de un DataSet.

**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```


Obtiene el DataSource. Generalmente es un objeto DataSet.

**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```


En modo de enlace de datos, indica si se deben crear encabezados de columnas vinculadas en la hoja.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtiene el índice de sí mismo dentro de las hojas de cálculo.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la hoja.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Obtiene el UniqueID en el Control

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control.

**Returns:**
boolean
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Agrupa filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a agrupar. |
| lastIndex | int | El índice de la última fila a agrupar. |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Agrupa filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a agrupar. |
| lastIndex | int | El índice de la última fila a agrupar. |
| isHidden | boolean | Especifica si las filas agrupadas están ocultas. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Obtiene si la hoja de cálculo está protegida. Cuando una hoja de cálculo está protegida, todas las celdas no pueden editarse excepto la celda cuya propiedad IsLocked es false.

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




### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Hace que todas las celdas sean editables. Este es un atributo extendido.

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Hace que todas las celdas sean de solo lectura. Este es un atributo extendido; tenga en cuenta que este atributo no se puede mantener en la celda real; si desea mantener la protección, por favor use setProtect.

### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```


En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar a la fuente de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```


En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar a la fuente de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```


Obtiene el número de filas vinculadas en modo de enlace de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```


Establece el DataMember del DataSource multi‑miembro. Generalmente representa un objeto DataTable de un DataSet.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```


Establece el DataSource. Generalmente es un objeto DataSet.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Hace que un rango de celdas sea editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Haga todas las celdas de solo lectura llamando al método SetAllCellsReadonly. Luego llame a este método para especificar el rango de celdas que debe ser editable

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial del rango. |
| startColumn | int | La columna inicial del rango. |
| filas | int | El número de filas. |
| columnas | int | El número de columnas. |

### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```


En modo de enlace de datos, indica si se deben crear encabezados de columnas vinculadas en la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre de la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```


Establece si la hoja de cálculo está protegida. Cuando una hoja de cálculo está protegida, todas las celdas no pueden editarse excepto la celda cuya propiedad IsLocked es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Hace que un rango de celdas sea de solo lectura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Primero haga todas las celdas editables llamando al método SetAllCellsEditable. Luego llame a este método para especificar el rango de celdas que debe ser de solo lectura

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial del rango. |
| startColumn | int | La columna inicial del rango. |
| filas | int | El número de filas. |
| columnas | int | El número de columnas. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unfreezePanes() {#unfreezePanes--}
```
public void unfreezePanes()
```


Descongela los paneles en la hoja de cálculo.

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Desagrupa filas.

**Remarks**

Solo elimina la información del grupo externo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a desagrupar. |
| lastIndex | int | El índice de la última fila a desagrupar. |

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

