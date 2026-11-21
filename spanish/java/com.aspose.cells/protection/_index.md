---
title: "Protección"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa los diversos tipos de opciones de protección disponibles para una hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

Representa los diversos tipos de opciones de protección disponibles para una hoja de cálculo.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Allowing users to select locked cells of the worksheet
         worksheet.getProtection().setAllowSelectingLockedCell(true);
         //Allowing users to select unlocked cells of the worksheet
         worksheet.getProtection().setAllowSelectingUnlockedCell(true);
```
## Métodos

| Método | Descripción |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | Copiar información de protección. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | Representa si se permite la eliminación de columnas en una hoja de cálculo protegida. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | Representa si se permite la eliminación de filas en una hoja de cálculo protegida. |
| [getAllowEditingContent()](#getAllowEditingContent--) | Representa si se permite al usuario editar el contenido de celdas bloqueadas en una hoja de cálculo protegida. |
| [getAllowEditingObject()](#getAllowEditingObject--) | Representa si se permite al usuario manipular objetos de dibujo en una hoja de cálculo protegida. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | Representa si se permite al usuario editar escenarios en una hoja de cálculo protegida. |
| [getAllowFiltering()](#getAllowFiltering--) | Representa si se permite al usuario utilizar un AutoFiltro que se creó antes de que la hoja estuviera protegida. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | Representa si se permite el formato de celdas en una hoja de cálculo protegida. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | Representa si se permite el formato de columnas en una hoja de cálculo protegida |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | Representa si se permite el formato de filas en una hoja de cálculo protegida |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | Representa si se permite la inserción de columnas en una hoja de cálculo protegida |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | Representa si la inserción de hipervínculos está permitida en una hoja de cálculo protegida |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | Representa si la inserción de filas está permitida en una hoja de cálculo protegida |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | Representa si el usuario puede seleccionar celdas bloqueadas en una hoja de cálculo protegida. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | Representa si el usuario puede seleccionar celdas desbloqueadas en una hoja de cálculo protegida. |
| [getAllowSorting()](#getAllowSorting--) | Representa si la opción de ordenación está permitida en una hoja de cálculo protegida. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | Representa si el usuario puede manipular tablas dinámicas en una hoja de cálculo protegida. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Representa la contraseña para proteger la hoja de cálculo. |
| [getPasswordHash()](#getPasswordHash--) | Obtiene el hash de la contraseña actual. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Indica si la hoja de cálculo está protegida con contraseña. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | Representa si se permite la eliminación de columnas en una hoja de cálculo protegida. |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | Representa si se permite la eliminación de filas en una hoja de cálculo protegida. |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | Representa si se permite al usuario editar el contenido de celdas bloqueadas en una hoja de cálculo protegida. |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | Representa si se permite al usuario manipular objetos de dibujo en una hoja de cálculo protegida. |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | Representa si se permite al usuario editar escenarios en una hoja de cálculo protegida. |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | Representa si se permite al usuario utilizar un AutoFiltro que se creó antes de que la hoja estuviera protegida. |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | Representa si se permite el formato de celdas en una hoja de cálculo protegida. |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | Representa si se permite el formato de columnas en una hoja de cálculo protegida |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | Representa si se permite el formato de filas en una hoja de cálculo protegida |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | Representa si se permite la inserción de columnas en una hoja de cálculo protegida |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | Representa si la inserción de hipervínculos está permitida en una hoja de cálculo protegida |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | Representa si la inserción de filas está permitida en una hoja de cálculo protegida |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | Representa si el usuario puede seleccionar celdas bloqueadas en una hoja de cálculo protegida. |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | Representa si el usuario puede seleccionar celdas desbloqueadas en una hoja de cálculo protegida. |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | Representa si la opción de ordenación está permitida en una hoja de cálculo protegida. |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | Representa si el usuario puede manipular tablas dinámicas en una hoja de cálculo protegida. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Representa la contraseña para proteger la hoja de cálculo. |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | Verifica la contraseña. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


Copiar información de protección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


Representa si se permite la eliminación de columnas en una hoja de cálculo protegida.

**Remarks**

Las columnas que contienen las celdas a eliminar deben estar desbloqueadas cuando la hoja está protegida, y la opción "Seleccionar celdas desbloqueadas" debe estar habilitada.

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


Representa si se permite la eliminación de filas en una hoja de cálculo protegida.

**Remarks**

Las filas que contienen las celdas a eliminar deben estar desbloqueadas cuando la hoja está protegida, y la opción "Seleccionar celdas desbloqueadas" debe estar habilitada.

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


Representa si se permite al usuario editar el contenido de celdas bloqueadas en una hoja de cálculo protegida.

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


Representa si se permite al usuario manipular objetos de dibujo en una hoja de cálculo protegida.

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


Representa si se permite al usuario editar escenarios en una hoja de cálculo protegida.

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


Representa si se permite al usuario utilizar un AutoFiltro que se creó antes de que la hoja estuviera protegida.

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


Representa si se permite el formato de celdas en una hoja de cálculo protegida.

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


Representa si se permite el formato de columnas en una hoja de cálculo protegida

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


Representa si se permite el formato de filas en una hoja de cálculo protegida

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


Representa si se permite la inserción de columnas en una hoja de cálculo protegida

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


Representa si la inserción de hipervínculos está permitida en una hoja de cálculo protegida

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


Representa si la inserción de filas está permitida en una hoja de cálculo protegida

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


Representa si el usuario puede seleccionar celdas bloqueadas en una hoja de cálculo protegida.

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


Representa si el usuario puede seleccionar celdas desbloqueadas en una hoja de cálculo protegida.

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


Representa si la opción de ordenación está permitida en una hoja de cálculo protegida.

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


Representa si el usuario puede manipular tablas dinámicas en una hoja de cálculo protegida.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```


Representa la contraseña para proteger la hoja de cálculo.

**Remarks**

Si la contraseña se establece en null o cadena vacía, puedes desproteger la hoja de cálculo o el libro sin usar una contraseña. De lo contrario, debes especificar la contraseña para desproteger la hoja de cálculo o el libro.

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


Obtiene el hash de la contraseña actual.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Indica si la hoja de cálculo está protegida con contraseña.

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




### setAllowDeletingColumn(boolean value) {#setAllowDeletingColumn-boolean-}
```
public void setAllowDeletingColumn(boolean value)
```


Representa si se permite la eliminación de columnas en una hoja de cálculo protegida.

**Remarks**

Las columnas que contienen las celdas a eliminar deben estar desbloqueadas cuando la hoja está protegida, y la opción "Seleccionar celdas desbloqueadas" debe estar habilitada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


Representa si se permite la eliminación de filas en una hoja de cálculo protegida.

**Remarks**

Las filas que contienen las celdas a eliminar deben estar desbloqueadas cuando la hoja está protegida, y la opción "Seleccionar celdas desbloqueadas" debe estar habilitada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


Representa si se permite al usuario editar el contenido de celdas bloqueadas en una hoja de cálculo protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


Representa si se permite al usuario manipular objetos de dibujo en una hoja de cálculo protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


Representa si se permite al usuario editar escenarios en una hoja de cálculo protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


Representa si se permite al usuario utilizar un AutoFiltro que se creó antes de que la hoja estuviera protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


Representa si se permite el formato de celdas en una hoja de cálculo protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


Representa si se permite el formato de columnas en una hoja de cálculo protegida

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


Representa si se permite el formato de filas en una hoja de cálculo protegida

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


Representa si se permite la inserción de columnas en una hoja de cálculo protegida

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


Representa si la inserción de hipervínculos está permitida en una hoja de cálculo protegida

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


Representa si la inserción de filas está permitida en una hoja de cálculo protegida

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


Representa si el usuario puede seleccionar celdas bloqueadas en una hoja de cálculo protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


Representa si el usuario puede seleccionar celdas desbloqueadas en una hoja de cálculo protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


Representa si la opción de ordenación está permitida en una hoja de cálculo protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


Representa si el usuario puede manipular tablas dinámicas en una hoja de cálculo protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Representa la contraseña para proteger la hoja de cálculo.

**Remarks**

Si la contraseña se establece en null o cadena vacía, puedes desproteger la hoja de cálculo o el libro sin usar una contraseña. De lo contrario, debes especificar la contraseña para desproteger la hoja de cálculo o el libro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(String password) {#verifyPassword-java.lang.String-}
```
public boolean verifyPassword(String password)
```


Verifica la contraseña.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| password | java.lang.String | La contraseña. |

**Returns:**
boolean -
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

