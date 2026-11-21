---
title: "AboveAverage"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Describe la regla de formato condicional AboveAverage."
type: docs
url: /es/java/com.aspose.cells/aboveaverage/
---

**Inheritance:**
java.lang.Object
```
public class AboveAverage
```

Describe la regla de formato condicional AboveAverage. Esta regla de formato condicional resalta las celdas que están por encima o por debajo del promedio de todos los valores en el rango.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AboveAverage()](#AboveAverage--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getStdDev()](#getStdDev--) | Obtiene el número de desviaciones estándar que se incluyen por encima o por debajo del promedio en la regla de formato condicional. |
| [hashCode()](#hashCode--) |  |
| [isAboveAverage()](#isAboveAverage--) | Obtiene la bandera que indica si la regla es una regla "above average". |
| [isEqualAverage()](#isEqualAverage--) | Obtiene la bandera que indica si los criterios 'aboveAverage' y 'belowAverage' son inclusivos del propio promedio, o exclusivos de ese valor. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAboveAverage(boolean value)](#setAboveAverage-boolean-) | Establece la bandera que indica si la regla es una regla "above average". |
| [setEqualAverage(boolean value)](#setEqualAverage-boolean-) | Establece la bandera que indica si los criterios 'aboveAverage' y 'belowAverage' son inclusivos del promedio mismo, o exclusivos de ese valor. |
| [setStdDev(int value)](#setStdDev-int-) | Establece el número de desviaciones estándar que se incluirán por encima o por debajo del promedio en la regla de formato condicional. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AboveAverage() {#AboveAverage--}
```
public AboveAverage()
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
### getStdDev() {#getStdDev--}
```
public int getStdDev()
```


Obtiene el número de desviaciones estándar que se incluirán por encima o por debajo del promedio en la regla de formato condicional. El valor de entrada debe estar entre 0 y 3 (incluyendo 0 y 3). Establecer este valor en 0 significa que stdDev no está configurado. El valor predeterminado es 0.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAboveAverage() {#isAboveAverage--}
```
public boolean isAboveAverage()
```


Obtiene la bandera que indica si la regla es una regla \"above average\". 'true' indica 'above average'. El valor predeterminado es true.

**Returns:**
boolean
### isEqualAverage() {#isEqualAverage--}
```
public boolean isEqualAverage()
```


Obtiene la bandera que indica si los criterios 'aboveAverage' y 'belowAverage' son inclusivos del promedio mismo, o exclusivos de ese valor. 'true' indica incluir el valor promedio en el criterio. El valor predeterminado es false.

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




### setAboveAverage(boolean value) {#setAboveAverage-boolean-}
```
public void setAboveAverage(boolean value)
```


Establece la bandera que indica si la regla es una regla \"above average\". 'true' indica 'above average'. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEqualAverage(boolean value) {#setEqualAverage-boolean-}
```
public void setEqualAverage(boolean value)
```


Establece la bandera que indica si los criterios 'aboveAverage' y 'belowAverage' son inclusivos del promedio mismo, o exclusivos de ese valor. 'true' indica incluir el valor promedio en el criterio. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStdDev(int value) {#setStdDev-int-}
```
public void setStdDev(int value)
```


Establece el número de desviaciones estándar que se incluirán por encima o por debajo del promedio en la regla de formato condicional. El valor de entrada debe estar entre 0 y 3 (incluyendo 0 y 3). Establecer este valor en 0 significa que stdDev no está configurado. El valor predeterminado es 0.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

