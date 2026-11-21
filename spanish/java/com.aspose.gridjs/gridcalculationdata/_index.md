---
title: "GridCalculationData"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa los datos requeridos al calcular una función, como los parámetros del nombre de la función ...etc."
type: docs
url: /es/java/com.aspose.gridjs/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Representa los datos requeridos al calcular una función, como el nombre de la función, los parámetros, etc.

**Remarks**

Todos los objetos proporcionados por esta clase son solo para propósito de "lectura". El usuario no debe cambiar ningún dato en el Workbook durante el proceso de cálculo de fórmulas, de lo contrario pueden producirse resultados inesperados o excepciones.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Obtiene el valor calculado para esta función. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtiene el índice de columna de la celda donde se encuentra la función. |
| [getFormula()](#getFormula--) | Obtiene la fórmula de la celda donde se encuentra la función. |
| [getFunctionName()](#getFunctionName--) | Obtiene el nombre de la función a calcular. |
| [getParamCount()](#getParamCount--) | Obtiene la cantidad de parámetros. |
| [getParamText(int index)](#getParamText-int-) | Obtiene el texto literal del parámetro en el índice dado. |
| [getParamValue(int index)](#getParamValue-int-) | Obtiene el objeto de valor representado del parámetro en el índice dado. |
| [getRow()](#getRow--) | Obtiene el índice de fila de la celda donde se encuentra la función. |
| [getSheetName()](#getSheetName--) | Obtiene el nombre de la hoja de cálculo donde se encuentra la función. |
| [getStringValue()](#getStringValue--) | Obtiene el DisplayStringValue de la celda donde se encuentra la función. |
| [getValue()](#getValue--) | Obtiene el valor de la celda donde se encuentra la función. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | Establece el valor calculado para esta función. |
| [toString()](#toString--) |  |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Obtiene el valor calculado para esta función.

**Remarks**

El usuario debe establecer esta propiedad en su motor de cálculo personalizado para aquellas funciones que el motor admite, y el valor establecido se devolverá al obtener esta propiedad. Obtener esta propiedad antes de establecerla hará que la función sea calculada por el motor de cálculo predeterminado de Aspose.Cells y se devolverá el valor calculado.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtiene el índice de columna de la celda donde se encuentra la función.

**Returns:**
int
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtiene la fórmula de la celda donde se encuentra la función.

**Returns:**
java.lang.String
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


Obtiene el nombre de la función a calcular.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


Obtiene la cantidad de parámetros.

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Obtiene el texto literal del parámetro en el índice dado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice del parámetro (basado en 0). |

**Returns:**
java.lang.String - El texto literal del parámetro.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Obtiene el objeto de valor representado del parámetro en el índice dado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice del parámetro (basado en 0). |

**Returns:**
java.lang.Object - Si el parámetro es un valor simple, entonces devuelve el valor simple. Si el parámetro es una referencia, entonces devuelve un objeto ReferredArea.
### getRow() {#getRow--}
```
public int getRow()
```


Obtiene el índice de fila de la celda donde se encuentra la función.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Obtiene el nombre de la hoja de cálculo donde se encuentra la función.

**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Obtiene el DisplayStringValue de la celda donde se encuentra la función.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Obtiene el valor de la celda donde se encuentra la función.

**Returns:**
java.lang.Object
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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


Establece el valor calculado para esta función.

**Remarks**

El usuario debe establecer esta propiedad en su motor de cálculo personalizado para aquellas funciones que el motor admite, y el valor establecido se devolverá al obtener esta propiedad. Obtener esta propiedad antes de establecerla hará que la función sea calculada por el motor de cálculo predeterminado de Aspose.Cells y se devolverá el valor calculado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

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

