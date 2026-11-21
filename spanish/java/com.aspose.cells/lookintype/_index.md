---
title: "LookInType"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el tipo de inspección."
type: docs
url: /es/java/com.aspose.cells/lookintype/
---

**Inheritance:**
java.lang.Object
```
public final class LookInType
```

Representa el tipo de inspección.
## Campos

| Campo | Descripción |
| --- | --- |
| [COMMENTS](#COMMENTS) | Encuentra el objeto solo desde el comentario de la celda. |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | Encuentra el objeto solo desde el valor formateado de la celda([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [FORMULAS](#FORMULAS) | Encuentra el objeto buscado desde la fórmula([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) si la celda es una fórmula, de lo contrario lo encuentra desde el valor original de la celda (igual que [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)). |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | Ignora celdas que no son fórmulas. |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | Buscar objeto solo a partir del valor original de la celda. |
| [VALUES](#VALUES) | Encuentra el objeto a partir del valor original de la celda([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) y del valor formateado([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | Ignora celdas que son fórmulas. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### COMMENTS {#COMMENTS}
```
public static final int COMMENTS
```


Encuentra el objeto solo a partir del comentario de la celda. Ignora aquellas celdas que no tienen comentario.

### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```


Encuentra el objeto solo desde el valor formateado de la celda([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```


Encuentra el objeto buscado desde la fórmula([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) si la celda es una fórmula, de lo contrario lo encuentra desde el valor original de la celda (igual que [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)).

### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```


Ignora celdas que no son fórmulas. Para esas celdas que son fórmulas, encuentra el objeto buscado a partir de la fórmula([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)).

### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```


Buscar objeto solo a partir del valor original de la celda.

### VALUES {#VALUES}
```
public static final int VALUES
```


Encuentra el objeto a partir del valor original de la celda([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) y del valor formateado([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```


Ignora celdas que son fórmulas. Para esas celdas que no son fórmulas, es lo mismo que [VALUES](../../com.aspose.cells/lookintype\#VALUES).

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

