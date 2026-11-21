---
title: "FormatConditionType"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Tipo de regla de formato condicional."
type: docs
url: /es/java/com.aspose.cells/formatconditiontype/
---

**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```

Tipo de regla de formato condicional.
## Campos

| Campo | Descripción |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | Esta regla de formato condicional resalta las celdas que están por encima o por debajo del promedio de todos los valores en el rango. |
| [BEGINS_WITH](#BEGINS-WITH) | Esta regla de formato condicional resalta las celdas en el rango que comienzan con el texto especificado. |
| [CELL_VALUE](#CELL-VALUE) | Esta regla de formato condicional compara el valor de una celda con el resultado calculado de una fórmula, usando un operador. |
| [COLOR_SCALE](#COLOR-SCALE) | Esta regla de formato condicional crea una escala de colores graduada en las celdas. |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | Esta regla de formato condicional resalta las celdas que están completamente vacías. |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | Esta regla de formato condicional resalta las celdas con errores de fórmula. |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | Esta regla de formato condicional resalta las celdas que contienen el texto especificado. |
| [DATA_BAR](#DATA-BAR) | Esta regla de formato condicional muestra una barra de datos graduada en el rango de celdas. |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | Esta regla de formato condicional resalta los valores duplicados. |
| [ENDS_WITH](#ENDS-WITH) | Esta regla de formato condicional resalta las celdas que terminan con el texto especificado. |
| [EXPRESSION](#EXPRESSION) | Esta regla de formato condicional contiene una fórmula para evaluar. |
| [ICON_SET](#ICON-SET) | Esta regla de formato condicional aplica íconos a las celdas según sus valores. |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | Esta regla de formato condicional resalta las celdas que no están vacías. |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | Esta regla de formato condicional resalta las celdas sin errores de fórmula. |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | Esta regla de formato condicional resalta las celdas que no contienen el texto especificado. |
| [TIME_PERIOD](#TIME-PERIOD) | Esta regla de formato condicional resalta las celdas que contienen fechas en el período de tiempo especificado. |
| [TOP_10](#TOP-10) | Esta regla de formato condicional resalta las celdas cuyos valores se encuentran en el rango superior N o inferior N, según se especifique. |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | Esta regla de formato condicional resalta los valores únicos en el rango. |
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
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```


Esta regla de formato condicional resalta las celdas que están por encima o por debajo del promedio de todos los valores en el rango.

### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```


Esta regla de formato condicional resalta las celdas en el rango que comienzan con el texto especificado. Equivalente a usar la función de hoja LEFT() y comparar valores.

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Esta regla de formato condicional compara el valor de una celda con el resultado calculado de una fórmula, usando un operador.

### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```


Esta regla de formato condicional crea una escala de colores graduada en las celdas.

### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```


Esta regla de formato condicional resalta las celdas que están completamente vacías. Equivalente a usar LEN(TRIM()). Esto significa que si la celda contiene solo caracteres que TRIM() eliminaría, se considera vacía. Una celda vacía también se considera vacía.

### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```


Esta regla de formato condicional resalta las celdas con errores de fórmula. Equivalente a usar la función de hoja ISERROR() para determinar si hay un error de fórmula.

### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```


Esta regla de formato condicional resalta las celdas que contienen el texto especificado. Equivalente a usar la función de hoja SEARCH() para determinar si la celda contiene el texto.

### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```


Esta regla de formato condicional muestra una barra de datos graduada en el rango de celdas.

### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```


Esta regla de formato condicional resalta los valores duplicados.

### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```


Esta regla de formato condicional resalta las celdas que terminan con el texto especificado. Equivalente a usar la función de hoja RIGHT() y comparar valores.

### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```


Esta regla de formato condicional contiene una fórmula para evaluar. Cuando el resultado de la fórmula es verdadero, la celda se resalta.

### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```


Esta regla de formato condicional aplica íconos a las celdas según sus valores.

### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```


Esta regla de formato condicional resalta celdas que no están vacías. Equivalente a usar LEN(TRIM()). Esto significa que si la celda contiene solo caracteres que TRIM() eliminaría, entonces se considera vacía. Una celda vacía también se considera vacía.

### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```


Esta regla de formato condicional resalta celdas sin errores de fórmula. Equivalente a usar la función de hoja ISERROR() para determinar si hay un error de fórmula.

### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```


Esta regla de formato condicional resalta celdas que no contienen el texto dado. Equivalente a usar la función de hoja SEARCH() para determinar si la celda contiene el texto o no.

### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```


Esta regla de formato condicional resalta celdas que contienen fechas en el período de tiempo especificado. El valor subyacente de la celda se evalúa, por lo que la celda no necesita estar formateada como fecha para ser evaluada. Por ejemplo, con una celda que contiene el valor 38913, el formato condicional se aplicará si la regla requiere un valor de 14/7/2006.

### TOP_10 {#TOP-10}
```
public static final int TOP_10
```


Esta regla de formato condicional resalta las celdas cuyos valores se encuentran en el rango superior N o inferior N, según se especifique.

### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```


Esta regla de formato condicional resalta los valores únicos en el rango.

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

