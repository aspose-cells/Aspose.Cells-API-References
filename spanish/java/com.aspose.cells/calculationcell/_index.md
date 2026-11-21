---
title: "CalculationCell"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa los datos relevantes del cálculo sobre una celda que se está calculando."
type: docs
url: /es/java/com.aspose.cells/calculationcell/
---

**Inheritance:**
java.lang.Object
```
public class CalculationCell
```

Representa los datos relevantes del cálculo sobre una celda que se está calculando.

**Remarks**

El usuario no debe cambiar ningún dato en el Libro de trabajo durante el proceso de cálculo de fórmulas, de lo contrario pueden producirse resultados inesperados o excepciones. Por lo tanto, todos los objetos proporcionados por esta clase (como el objeto Cell de [getCell()](../../com.aspose.cells/calculationcell\#getCell--)) son solo para fines de "lectura".
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Obtiene el objeto Cell que está siendo calculado. |
| [getCellColumn()](#getCellColumn--) | Obtiene el índice de columna de la celda. |
| [getCellRow()](#getCellRow--) | Obtiene el índice de fila de la celda. |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | Obtiene el objeto Workbook. |
| [getWorksheet()](#getWorksheet--) | Obtiene el objeto Worksheet donde se encuentra la celda. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | Establece el valor calculado para la celda. |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


Obtiene el objeto Cell que está siendo calculado.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Obtiene el índice de columna de la celda.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Obtiene el índice de fila de la celda.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtiene el objeto Workbook.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtiene el objeto Worksheet donde se encuentra la celda.

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




### setCalculatedValue(Object v) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object v)
```


Establece el valor calculado para la celda.

**Remarks**

El usuario puede establecer el resultado calculado mediante este método para ignorar el cálculo automático de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| v | java.lang.Object |  |

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

