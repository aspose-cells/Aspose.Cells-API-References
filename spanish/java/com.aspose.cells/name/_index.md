---
title: "Name"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una colección de todos los objetos [Name](../com.aspose.cells/name) en la hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/name/
---

**Inheritance:**
java.lang.Object
```
public class Name
```

Representa una colección de todos los objetos [Name](../com.aspose.cells/name) en la hoja de cálculo.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating a named range
         Range range = worksheet.getCells().createRange("B4", "G14");
         //Setting the name of the named range
         range.setName("TestRange");
         //Saving the modified Excel file in default (that is Excel 2000) format
         workbook.save("output.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Obtiene el comentario del nombre. |
| [getFullText()](#getFullText--) | Obtiene el texto completo del nombre del objeto con la configuración de alcance. |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | Obtiene una referencia R1C1 del [Name](../../com.aspose.cells/name). |
| [getRange()](#getRange--) | Obtiene el rango si este nombre se refiere a un rango. |
| [getRange(boolean recalculate)](#getRange-boolean-) | Obtiene el rango si este nombre se refiere a un rango |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | Obtiene el rango si este nombre se refiere a un rango. |
| [getRanges()](#getRanges--) | Obtiene todos los rangos referidos por este nombre. |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | Obtiene todos los rangos referidos por este nombre. |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | Obtiene todas las referencias referidas por este nombre. |
| [getRefersTo()](#getRefersTo--) | Devuelve o establece la fórmula a la que el nombre está definido para referirse, comenzando con un signo igual. |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | Obtener la referencia de este Nombre. |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | Obtener la referencia de este Nombre basado en la celda especificada. |
| [getSheetIndex()](#getSheetIndex--) | Indica que este nombre pertenece a Workbook o Worksheet. 0 = nombre global, de lo contrario índice a la hoja (basado en uno). |
| [getText()](#getText--) | Obtiene el texto del nombre del objeto. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Indica si este nombre es referenciado por otras fórmulas. |
| [isVisible()](#isVisible--) | Indica si el nombre es visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | Establece el comentario del nombre. |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | Establece una referencia R1C1 del [Name](../../com.aspose.cells/name). |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | Devuelve o establece la fórmula a la que el nombre está definido para referirse, comenzando con un signo igual. |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | Establece la referencia de este Nombre. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | Indica que este nombre pertenece a Workbook o Worksheet. 0 = nombre global, de lo contrario índice a la hoja (basado en uno). |
| [setText(String value)](#setText-java.lang.String-) | Obtiene el texto del nombre del objeto. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica si el nombre es visible. |
| [toString()](#toString--) | Devuelve una cadena que representa el objeto Range actual. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getComment() {#getComment--}
```
public String getComment()
```


Obtiene el comentario del nombre. Solo se aplica a Excel 2007 o versiones superiores.

**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```


Obtiene el texto completo del nombre del objeto con la configuración de alcance.

**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```


Obtiene una referencia R1C1 del [Name](../../com.aspose.cells/name).

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Obtiene el rango si este nombre se refiere a un rango.

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```


Obtiene el rango si este nombre se refiere a un rango

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recalcular | boolean | si recalcularlo si este nombre ya ha sido calculado antes de esta invocación. |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```


Obtiene el rango si este nombre se refiere a un rango. Si la referencia de este nombre no es absoluta, el rango puede ser diferente para cada celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | El índice de hoja correspondiente. |
| fila | int | El índice de fila correspondiente. |
| columna | int | El índice de columna correspondiente |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Obtiene todos los rangos referidos por este nombre.

**Returns:**
com.aspose.cells.Range[] - Todos los rangos.
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```


Obtiene todos los rangos referidos por este nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recalcular | boolean | si recalcularlo si este nombre ya ha sido calculado antes de esta invocación. |

**Returns:**
com.aspose.cells.Range[] - Todos los rangos.
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```


Obtiene todas las referencias referidas por este nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recalcular | boolean | si recalcularlo si este nombre ya ha sido calculado antes de esta invocación. |

**Returns:**
com.aspose.cells.ReferredArea[] - Todos los rangos.
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Devuelve o establece la fórmula a la que el nombre está definido para referirse, comenzando con un signo igual.

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```


Obtener la referencia de este Nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la referencia necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la referencia necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtener la referencia de este Nombre basado en la celda especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la referencia necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la referencia necesita formatearse según la configuración regional. |
| fila | int | El índice de fila de la celda. |
| columna | int | El índice de columna de la celda. |

**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Indica que este nombre pertenece a Workbook o Worksheet. 0 = nombre global, de lo contrario índice a la hoja (basado en uno).

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Obtiene el texto del nombre del objeto.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Indica si este nombre es referenciado por otras fórmulas.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indica si el nombre es visible.

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




### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Establece el comentario del nombre. Solo se aplica a Excel 2007 o versiones superiores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```


Establece una referencia R1C1 del [Name](../../com.aspose.cells/name).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```


Devuelve o establece la fórmula a la que el nombre está definido para referirse, comenzando con un signo igual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```


Establece la referencia de este Nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| refersTo | java.lang.String | La referencia. |
| isR1C1 | boolean | Indica si la referencia está en formato R1C1. |
| isLocal | boolean | Si la referencia está formateada según la configuración regional. |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


Indica que este nombre pertenece a Workbook o Worksheet. 0 = nombre global, de lo contrario índice a la hoja (basado en uno).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Obtiene el texto del nombre del objeto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica si el nombre es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa el objeto Range actual.

**Returns:**
java.lang.String -
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

