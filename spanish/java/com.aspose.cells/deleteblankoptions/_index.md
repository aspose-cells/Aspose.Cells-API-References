---
title: "DeleteBlankOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración de eliminación de celdas/filas/columnas en blanco."
type: docs
url: /es/java/com.aspose.cells/deleteblankoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```

Representa la configuración de eliminación de celdas/filas/columnas en blanco.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | Indica si los objetos relacionados con dibujos, como imágenes, formas, gráficos..., se considerarán en blanco. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | Si una celda se considerará en blanco cuando es una fórmula y el resultado calculado es nulo o una cadena vacía. |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | Indica si una celda se considerará en blanco cuando su valor es una cadena vacía. |
| [getEndIndex()](#getEndIndex--) | Especifica el índice de fila/columna final (inclusive) del rango a comprobar y eliminar filas/columnas en blanco. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | Obtiene el monitor para rastrear los cambios causados por la eliminación. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | Indica cómo procesar celdas combinadas al eliminar filas/columnas en blanco. |
| [getStartIndex()](#getStartIndex--) | Especifica el índice de fila/columna inicial del rango a comprobar y eliminar filas/columnas en blanco. |
| [getUpdateReference()](#getUpdateReference--) | Indica si actualizar referencias en otras hojas de cálculo. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | Indica si los objetos relacionados con dibujos, como imágenes, formas, gráficos..., se considerarán en blanco. |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | Si una celda se considerará en blanco cuando es una fórmula y el resultado calculado es nulo o una cadena vacía. |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | Indica si una celda se considerará en blanco cuando su valor es una cadena vacía. |
| [setEndIndex(int value)](#setEndIndex-int-) | Especifica el índice de fila/columna final (inclusive) del rango a comprobar y eliminar filas/columnas en blanco. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | Establece el monitor para rastrear los cambios causados por la eliminación. |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | Indica cómo procesar celdas combinadas al eliminar filas/columnas en blanco. |
| [setStartIndex(int value)](#setStartIndex-int-) | Especifica el índice de fila/columna inicial del rango a comprobar y eliminar filas/columnas en blanco. |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Indica si actualizar referencias en otras hojas de cálculo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```


Indica si los objetos relacionados con dibujos, como imágenes, formas, gráficos..., se considerarán en blanco. El valor predeterminado es true.

**Remarks**

Al establecer esta propiedad como false, todas las filas/columnas cubiertas por objetos de dibujo no se considerarán en blanco y no se eliminarán.

**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```


Si una celda se considerará en blanco cuando es una fórmula y el resultado calculado es nulo o una cadena vacía. El valor predeterminado es false.

**Remarks**

En general, el usuario debe asegurarse de que las fórmulas se hayan calculado antes de la operación de eliminación con esta propiedad establecida en true. De lo contrario, todas las fórmulas recién creadas mediante APIs normales como [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) se considerarán en blanco y pueden ser eliminadas porque, antes del cálculo, sus resultados calculados son todos nulos.

**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```


Indica si una celda se considerará en blanco cuando su valor es una cadena vacía. El valor predeterminado es true.

**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```


Especifica el índice de fila/columna final (inclusive) del rango a comprobar y eliminar filas/columnas en blanco. El valor predeterminado es -1 y -1 significa el rango máximo de todos los objetos (celdas, dibujos, ...) que deben revisarse.

**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```


Obtiene el monitor para rastrear los cambios causados por la eliminación.

**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```


Indica cómo procesar celdas combinadas al eliminar filas/columnas en blanco.

Ver [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Para [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY), todas las celdas en él se considerarán en blanco excepto la celda superior izquierda que no está en blanco. Es el valor predeterminado de esta propiedad.

Para [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE), todas las celdas en él se considerarán no en blanco.

Para [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT), todas las celdas fuera del área de visualización del contenido se considerarán en blanco.



**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Especifica el índice de fila/columna inicial del rango a comprobar y eliminar filas/columnas en blanco.

**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Indica si actualizar referencias en otras hojas de cálculo.

**Remarks**

A partir de la versión 26.7 establecemos el valor predeterminado de esta propiedad en true.

**Returns:**
boolean
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




### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```


Indica si los objetos relacionados con dibujos, como imágenes, formas, gráficos..., se considerarán en blanco. El valor predeterminado es true.

**Remarks**

Al establecer esta propiedad como false, todas las filas/columnas cubiertas por objetos de dibujo no se considerarán en blanco y no se eliminarán.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```


Si una celda se considerará en blanco cuando es una fórmula y el resultado calculado es nulo o una cadena vacía. El valor predeterminado es false.

**Remarks**

En general, el usuario debe asegurarse de que las fórmulas se hayan calculado antes de la operación de eliminación con esta propiedad establecida en true. De lo contrario, todas las fórmulas recién creadas mediante APIs normales como [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) se considerarán en blanco y pueden ser eliminadas porque, antes del cálculo, sus resultados calculados son todos nulos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```


Indica si una celda se considerará en blanco cuando su valor es una cadena vacía. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```


Especifica el índice de fila/columna final (inclusive) del rango a comprobar y eliminar filas/columnas en blanco. El valor predeterminado es -1 y -1 significa el rango máximo de todos los objetos (celdas, dibujos, ...) que deben revisarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```


Establece el monitor para rastrear los cambios causados por la eliminación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |

### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```


Indica cómo procesar celdas combinadas al eliminar filas/columnas en blanco.

Ver [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Para [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY), todas las celdas en él se considerarán en blanco excepto la celda superior izquierda que no está en blanco. Es el valor predeterminado de esta propiedad.

Para [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE), todas las celdas en él se considerarán no en blanco.

Para [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT), todas las celdas fuera del área de visualización del contenido se considerarán en blanco.



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```


Especifica el índice de fila/columna inicial del rango a comprobar y eliminar filas/columnas en blanco.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Indica si actualizar referencias en otras hojas de cálculo.

**Remarks**

A partir de la versión 26.7 establecemos el valor predeterminado de esta propiedad en true.

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

