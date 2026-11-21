---
title: "GridCalculationData"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa los datos requeridos al calcular una función, como los parámetros del nombre de la función ...etc."
type: docs
url: /es/java/com.aspose.gridweb/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Representa los datos requeridos al calcular una función, como el nombre de la función, los parámetros, etc.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Obtiene el valor calculado para esta función. |
| [getCell()](#getCell--) | Obtiene el objeto Cell donde se encuentra la función. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Obtiene el nombre de la función a calcular. |
| [getParamCount()](#getParamCount--) | Obtiene la cantidad de parámetros |
| [getParamText(int index)](#getParamText-int-) | Obtiene el texto literal del parámetro en el índice dado. |
| [getParamValue(int index)](#getParamValue-int-) | Obtiene el objeto de valor representado del parámetro en el índice dado. |
| [getWorkbook()](#getWorkbook--) | Obtiene el objeto Workbook donde se encuentra la función. |
| [getWorksheet()](#getWorksheet--) | Obtiene el objeto Workbook donde se encuentra la función. |
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
### getCell() {#getCell--}
```
public GridCell getCell()
```


Obtiene el objeto Cell donde se encuentra la función.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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


Obtiene la cantidad de parámetros

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
| índice | int | índice del parámetro (base 0) |

**Returns:**
java.lang.String - texto literal del parámetro.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Obtiene el objeto de valor representado del parámetro en el índice dado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | índice del parámetro (base 0) |

**Returns:**
java.lang.Object - Si el parámetro es un valor simple, entonces devuelve el valor simple. Si el parámetro es una referencia, entonces devuelve un objeto ReferredArea.
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Obtiene el objeto Workbook donde se encuentra la función.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getWorksheet() {#getWorksheet--}
```
public GridWorksheet getWorksheet()
```


Obtiene el objeto Workbook donde se encuentra la función.

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
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

