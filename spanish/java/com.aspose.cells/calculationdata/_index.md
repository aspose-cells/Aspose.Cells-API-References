---
title: "CalculationData"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa los datos requeridos al calcular una función, como los parámetros del nombre de la función ...etc."
type: docs
url: /es/java/com.aspose.cells/calculationdata/
---

**Inheritance:**
java.lang.Object
```
public class CalculationData
```

Representa los datos requeridos al calcular una función, como el nombre de la función, los parámetros, etc.

**Remarks**

Todos los objetos proporcionados por esta clase son solo para propósito de "lectura". El usuario no debe cambiar ningún dato en el Workbook durante el proceso de cálculo de fórmulas, de lo contrario pueden producirse resultados inesperados o excepciones.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Obtiene el valor calculado para esta función. |
| [getCell()](#getCell--) | Obtiene el objeto Cell donde está la función. |
| [getCellColumn()](#getCellColumn--) | Obtiene el índice de columna de la celda donde está la función. |
| [getCellRow()](#getCellRow--) | Obtiene el índice de fila de la celda donde está la función. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Obtiene el nombre de la función a calcular. |
| [getParamCount()](#getParamCount--) | Obtiene la cantidad de parámetros |
| [getParamText(int index)](#getParamText-int-) | Obtiene el texto literal del parámetro en el índice dado. |
| [getParamValue(int index)](#getParamValue-int-) | Obtiene el objeto de valor representado del parámetro en un índice dado. |
| [getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)](#getParamValueInArrayMode-int-int-int-) | Obtiene el(los) valor(es) del parámetro en un índice dado. |
| [getWorkbook()](#getWorkbook--) | Obtiene el objeto Workbook donde está la función. |
| [getWorksheet()](#getWorksheet--) | Obtiene el objeto Worksheet donde está la función. |
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

El usuario debe establecer esta propiedad en su motor de cálculo personalizado para aquellas funciones que el motor admite, y el valor establecido se devolverá al obtener esta propiedad más tarde. El valor establecido puede ser de tipos posibles de [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), o una matriz de ese tipo de valores, o un Range, Name, ReferredArea. Obtener esta propiedad antes de asignarle un valor hará que la función sea calculada por el motor de cálculo predeterminado de Aspose.Cells y luego se devolverá el valor calculado (generalmente debería ser \#NAME? para funciones definidas por el usuario).

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public Cell getCell()
```


Obtiene el objeto Cell donde está la función.

**Remarks**

Al calcular una fórmula sin asignarla a una celda, como mediante [Worksheet.calculateFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateFormula-String-CalculationOptions-), la fórmula se calculará como si se hubiera asignado a la celda A1, por lo que tanto [getCellRow()](../../com.aspose.cells/calculationdata\#getCellRow--) como [getCellColumn()](../../com.aspose.cells/calculationdata\#getCellColumn--) son 0. Sin embargo, la celda A1 en la hoja de cálculo puede no haber sido instanciada. Por lo tanto, para este tipo de situación esta propiedad será nula.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Obtiene el índice de columna de la celda donde está la función.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Obtiene el índice de fila de la celda donde está la función.

**Returns:**
int
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


Obtiene el objeto de valor representado del parámetro en un índice dado.

**Remarks**

Para un parámetro:

Si es un valor simple, entonces devuelve el propio valor simple;

Si es una referencia, entonces devuelve el objeto ReferredArea;

Si hace referencia a conjunto(s) de datos con múltiples valores, entonces devuelve una matriz de objetos;

Si es algún tipo de expresión que necesita ser calculada, entonces se calculará en modo valor y generalmente se devolverá un solo valor según la base de la celda actual. Por ejemplo, si un parámetro de la fórmula de D2 es A:A+B:B, entonces se calculará y devolverá A2+B2. Sin embargo, si este parámetro se ha especificado en modo matriz (por  o ), entonces se devolverá una matriz (object[][]) cuyos elementos son A1+B1, A2+B2, ....

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice del parámetro (base 0) |

**Returns:**
java.lang.Object - El valor calculado del parámetro.
### getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount) {#getParamValueInArrayMode-int-int-int-}
```
public Object[][] getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```


Obtiene el(los) valor(es) del parámetro en un índice dado. Si el parámetro es algún tipo de expresión que necesita ser calculada, entonces se calculará en modo matriz.

**Remarks**

Para una expresión que necesita ser calculada, tomando A:A+B:B como ejemplo: en modo valor se calculará a un solo valor según la base de la celda actual. Pero en modo matriz, se calcularán todos los valores de A1+B1, A2+B2, A3+B3, ... y se usarán para construir la matriz devuelta. Y para este tipo de situación, es mejor especificar el límite para el recuento de filas/columnas (por ejemplo, de acuerdo con [Cells.getMaxDataRow()](../../com.aspose.cells/cells\#getMaxDataRow--) y [Cells.getMaxDataColumn()](../../com.aspose.cells/cells\#getMaxDataColumn--)), de lo contrario la gran matriz devuelta puede aumentar el consumo de memoria con una gran cantidad de datos inútiles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice del parámetro (base 0) |
| maxRowCount | int | El límite de recuento de filas para la matriz devuelta. Si es no positivo o mayor que el recuento real de filas, se usará el recuento real de filas. |
| maxColumnCount | int | El límite de recuento de columnas para la matriz devuelta. Si es no positivo o mayor que el recuento real de filas, se usará el recuento real de columnas. |

**Returns:**
java.lang.Object[][] - Una matriz que contiene todos los elementos representados por el parámetro especificado.
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtiene el objeto Workbook donde está la función.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtiene el objeto Worksheet donde está la función.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

El usuario debe establecer esta propiedad en su motor de cálculo personalizado para aquellas funciones que el motor admite, y el valor establecido se devolverá al obtener esta propiedad más tarde. El valor establecido puede ser de tipos posibles de [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), o una matriz de ese tipo de valores, o un Range, Name, ReferredArea. Obtener esta propiedad antes de asignarle un valor hará que la función sea calculada por el motor de cálculo predeterminado de Aspose.Cells y luego se devolverá el valor calculado (generalmente debería ser \#NAME? para funciones definidas por el usuario).

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

