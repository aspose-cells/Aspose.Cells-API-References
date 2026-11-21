---
title: "ListColumn"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una columna en una tabla."
type: docs
url: /es/java/com.aspose.cells/listcolumn/
---

**Inheritance:**
java.lang.Object
```
public class ListColumn
```

Representa una columna en una tabla.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         ListColumn listColumn = table.getListColumns().get(4);
         listColumn.setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         listColumn.setFormula("=[A]");
         workbook.save("Book1.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | Obtiene la fórmula de esta columna de lista. |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | Obtiene la fórmula de la fila de totales de esta columna de lista. |
| [getDataStyle()](#getDataStyle--) | Obtiene el estilo de los datos en esta columna de la tabla. |
| [getFormula()](#getFormula--) | Obtiene la fórmula de la columna de lista. |
| [getName()](#getName--) | Obtiene el nombre de la columna. |
| [getRange()](#getRange--) | Obtiene el rango de esta columna de lista. |
| [getTotalsCalculation()](#getTotalsCalculation--) | Obtiene el tipo de cálculo en la fila Totales de la columna de lista. |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | Obtiene las etiquetas de visualización de la fila total. |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | Indica si la fórmula es una fórmula de matriz. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | Establece la fórmula para esta columna de lista. |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | Obtiene la fórmula de la fila de totales de esta columna de lista. |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | Establece el estilo de los datos en esta columna de la tabla. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Establece la fórmula de la columna de lista. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la columna. |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | Establece el tipo de cálculo en la fila Totales de la columna de lista. |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | Establece las etiquetas de visualización de la fila total. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomCalculatedFormula(boolean isR1C1, boolean isLocal) {#getCustomCalculatedFormula-boolean-boolean-}
```
public String getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)
```


Obtiene la fórmula de esta columna de lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String - La fórmula de esta columna de lista.
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```


Obtiene la fórmula de la fila de totales de esta columna de lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String - La fórmula de esta columna de lista.
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```


Obtiene el estilo de los datos en esta columna de la tabla.

**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtiene la fórmula de la columna de lista.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la columna.

**Remarks**

Si se establece el nombre de la columna, el valor de la celda correspondiente también se cambiará.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Obtiene el rango de esta columna de lista.

**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```


Obtiene el tipo de cálculo en la fila Totales de la columna de lista.

Ver [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```


Obtiene las etiquetas de visualización de la fila total.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Indica si la fórmula es una fórmula de matriz.

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




### setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomCalculatedFormula-java.lang.String-boolean-boolean-}
```
public void setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)
```


Establece la fórmula para esta columna de lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | la fórmula para esta columna de lista. |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```


Obtiene la fórmula de la fila de totales de esta columna de lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | la fórmula para esta columna de lista. |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```


Establece el estilo de los datos en esta columna de la tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Establece la fórmula de la columna de lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre de la columna.

**Remarks**

Si se establece el nombre de la columna, el valor de la celda correspondiente también se cambiará.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```


Establece el tipo de cálculo en la fila Totales de la columna de lista.

Ver [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```


Establece las etiquetas de visualización de la fila total.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

