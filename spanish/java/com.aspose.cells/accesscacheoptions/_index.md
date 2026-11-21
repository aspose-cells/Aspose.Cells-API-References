---
title: "AccessCacheOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Opciones de caché para el acceso a datos."
type: docs
url: /es/java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

Opciones de caché para el acceso a datos. Se pueden combinar múltiples opciones usando el operador "\|".

**Remarks**

Para algunas funciones, acceder a un conjunto de datos grande requiere muchas operaciones repetidas y complejas, como búsquedas, cálculos, ...etc, y esas operaciones consumen mucho tiempo adicional. En situaciones comunes, todos los datos dependientes permanecen sin cambios durante el acceso, por lo que se pueden crear y utilizar algunas cachés para mejorar el rendimiento del acceso. Con este fin, proporcionamos esta API para que el usuario pueda especificar qué tipo de acceso a datos necesita ser optimizado mediante un posible mecanismo de caché.

Tenga en cuenta que, para diferentes opciones, puede ser necesario que distintos conjuntos de datos sean "solo lectura". Además, el rendimiento del acceso a datos depende de muchos factores; el uso de un mecanismo de caché no garantiza que el rendimiento mejore. En algunas situaciones, como cuando el conjunto de datos a acceder es pequeño, usar caché puede incluso consumir más tiempo, ya que la propia caché también requiere tiempo adicional.
## Campos

| Campo | Descripción |
| --- | --- |
| [ALL](#ALL) | Aplicar todas las optimizaciones posibles para todo tipo de acceso a datos en el libro de trabajo. |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | Aplicar la optimización posible para el cálculo de fórmulas. |
| [CELLS_DATA](#CELLS-DATA) | Aplicar la optimización posible para obtener los valores de las celdas. |
| [CELL_DISPLAY](#CELL-DISPLAY) | Aplicar la optimización posible para obtener los resultados relacionados con la visualización de las celdas([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), etc.). |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Aplicar la optimización posible para obtener el resultado de formato de los formatos condicionales. |
| [GET_FORMULA](#GET-FORMULA) | Aplicar la optimización posible para obtener fórmulas. |
| [NONE](#NONE) | Sin caché para ningún acceso a datos. |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | Aplicar la optimización posible para obtener la posición y el tamaño del objeto (como Shape). |
| [SET_FORMULA](#SET-FORMULA) | Aplicar la optimización posible para establecer fórmulas. |
| [VALIDATION](#VALIDATION) | Aplicar la optimización posible para obtener el resultado de validación. |
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
### ALL {#ALL}
```
public static final int ALL
```


Aplicar todas las optimizaciones posibles para todo tipo de acceso a datos en el libro de trabajo. Todas las configuraciones y datos no deben modificarse durante el acceso optimizado.

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


Aplicar la optimización posible para el cálculo de fórmulas. Los datos de las celdas no deben modificarse durante el acceso optimizado, tampoco deben crearse nuevos objetos (Cell, Row, etc.) (por ejemplo mediante [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


Aplicar la optimización posible para obtener los valores de las celdas. Los datos de las celdas (datos y configuraciones de Cell, Row) no deben modificarse durante el acceso optimizado, tampoco deben crearse nuevos objetos Cell/Row (por ejemplo mediante [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


Aplicar la optimización posible para obtener los resultados relacionados con la visualización de las celdas([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), etc.). Los datos de las celdas y los objetos relacionados con el estilo (estilos de Cell/Row/Column, ancho de columna, etc.) no deben modificarse durante el acceso optimizado.

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Aplicar la posible optimización para obtener el resultado de formato de los formatos condicionales. Todos los datos y configuraciones que puedan afectar el resultado de los formatos condicionales (configuraciones de formatos condicionales, valores de celdas dependientes, etc.) no deben cambiarse durante el acceso optimizado.

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


Aplicar la posible optimización para obtener fórmulas. Todos los datos y configuraciones que puedan afectar la expresión de la fórmula (nombre de la hoja de cálculo, texto del nombre, columna de la tabla, etc.) no deben cambiarse durante el acceso optimizado.

### NONE {#NONE}
```
public static final int NONE
```


Sin caché para ningún acceso a datos.

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


Aplicar la posible optimización para obtener la posición y el tamaño del objeto (como una Forma). Las configuraciones de altura de fila y ancho de columna no deben cambiarse durante el acceso optimizado.

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


Aplicar la posible optimización para establecer fórmulas. Todos los datos y configuraciones que puedan afectar la expresión de la fórmula (nombre de la hoja de cálculo, texto del nombre, columna de la tabla, etc.) no deben cambiarse durante el acceso optimizado.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Aplicar la posible optimización para obtener el resultado de validación. Todos los datos y configuraciones que puedan afectar el resultado de la validación (configuraciones de la validación, valores de celdas dependientes, etc.) no deben cambiarse durante el acceso optimizado.

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

