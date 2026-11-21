---
title: "FormatCondition"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la condición de formato condicional."
type: docs
url: /es/java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

Representa la condición de formato condicional.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
 
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
 
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
 
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         //Saving the Excel file
         workbook.save("output.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | Obtén la instancia "AboveAverage" del formato condicional. |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | Obtén la instancia "ColorScale" del formato condicional. |
| [getDataBar()](#getDataBar--) | Obtén la instancia "DataBar" del formato condicional. |
| [getFormula1()](#getFormula1--) | Obtiene el valor o expresión asociado al formato condicional. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Obtiene el valor o expresión asociado a esta condición de formato. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Obtiene el valor o expresión del formato condicional de la celda. |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | Obtiene la fórmula del formato condicional de la celda. |
| [getFormula2()](#getFormula2--) | Obtiene el valor o expresión asociado al formato condicional. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Obtiene el valor o expresión asociado a esta condición de formato. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Obtiene el valor o expresión del formato condicional de la celda. |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | Obtiene la fórmula del formato condicional de la celda. |
| [getIconSet()](#getIconSet--) | Obtén la instancia "IconSet" del formato condicional. |
| [getOperator()](#getOperator--) | Obtiene el tipo de operador del formato condicional. |
| [getPriority()](#getPriority--) | La prioridad de esta regla de formato condicional. |
| [getStopIfTrue()](#getStopIfTrue--) | Verdadero, no se pueden aplicar reglas con menor prioridad sobre esta regla, cuando esta regla evalúa a verdadero. |
| [getStyle()](#getStyle--) | Obtiene o establece el estilo de los rangos de celdas con formato condicional. |
| [getText()](#getText--) | El valor de texto en una regla de formato condicional "text contains". |
| [getTimePeriod()](#getTimePeriod--) | El período de tiempo aplicable en una regla de formato condicional "date occurrin". |
| [getTop10()](#getTop10--) | Obtén la instancia "Top10" del formato condicional. |
| [getType()](#getType--) | Obtiene si el tipo de formato condicional. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Establece el valor o expresión asociado al formato condicional. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Establece el valor o expresión asociado a esta condición de formato. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Establece el valor o expresión asociado al formato condicional. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Establece el valor o expresión asociado a esta condición de formato. |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | Establece el valor o expresión asociado a esta condición de formato. |
| [setOperator(int value)](#setOperator-int-) | Establece el tipo de operador del formato condicional. |
| [setPriority(int value)](#setPriority-int-) | La prioridad de esta regla de formato condicional. |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | Verdadero, no se pueden aplicar reglas con menor prioridad sobre esta regla, cuando esta regla evalúa a verdadero. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Obtiene o establece el estilo de los rangos de celdas con formato condicional. |
| [setText(String value)](#setText-java.lang.String-) | El valor de texto en una regla de formato condicional "text contains". |
| [setTimePeriod(int value)](#setTimePeriod-int-) | El período de tiempo aplicable en una regla de formato condicional "date occurrin". |
| [setType(int value)](#setType-int-) | Establece si el tipo de formato condicional. |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


Obtén la instancia "AboveAverage" del formato condicional. La regla de la instancia predeterminada resalta las celdas que están por encima del promedio de todos los valores en el rango. Válido solo para type = AboveAverage.

**Returns:**
[AboveAverage](../../com.aspose.cells/aboveaverage) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorScale() {#getColorScale--}
```
public ColorScale getColorScale()
```


Obtén la instancia "ColorScale" del formato condicional. La instancia predeterminada es una "green-yellow-red" 3ColorScale. Válido solo para type = ColorScale.

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


Obtén la instancia "DataBar" del formato condicional. El color de la instancia predeterminada es azul. Válido solo para type = DataBar.

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Obtiene el valor o expresión asociado al formato condicional.

**Remarks**

Por favor, añada todas las áreas antes de establecer la fórmula. Para establecer la fórmula de esta condición, si el valor de entrada comienza con '=', se tomará como fórmula. De lo contrario se tomará como valor simple (texto, número, bool). Para valores de texto que comienzan con '=', el usuario puede ingresarlos como fórmula en el formato: "=\\\"=...\\\"".

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Obtiene el valor o expresión asociado a esta condición de formato.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String - El valor o expresión asociado a esta condición de formato.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtiene el valor o expresión del formato condicional de la celda.

**Remarks**

La celda dada debe estar contenida por este formato condicional, de lo contrario se devolverá null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
java.lang.String - El valor o expresión asociado al formato condicional de la celda.
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


Obtiene la fórmula del formato condicional de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
java.lang.String - La fórmula.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Obtiene el valor o expresión asociado al formato condicional.

**Remarks**

Por favor, añada todas las áreas antes de establecer la fórmula. Para establecer la fórmula de esta condición, si el valor de entrada comienza con '=', se tomará como fórmula. De lo contrario se tomará como valor simple (texto, número, bool). Para valores de texto que comienzan con '=', el usuario puede ingresarlos como fórmula en el formato: "=\\\"=...\\\"".

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Obtiene el valor o expresión asociado a esta condición de formato.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String - El valor o expresión asociado a esta condición de formato.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtiene el valor o expresión del formato condicional de la celda.

**Remarks**

La celda dada debe estar contenida por este formato condicional, de lo contrario se devolverá null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
java.lang.String - El valor o expresión asociado al formato condicional de la celda.
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


Obtiene la fórmula del formato condicional de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
java.lang.String - La fórmula.
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


Obtén la instancia "IconSet" del formato condicional. El IconSetType de la instancia predeterminada es TrafficLights31. Válido solo para type = IconSet.

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


Obtiene el tipo de operador del formato condicional.

Ver [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


La prioridad de esta regla de formato condicional. Este valor se usa para determinar qué formato debe evaluarse y renderizarse. Los valores numéricos más bajos tienen mayor prioridad que los valores numéricos más altos, donde '1' es la prioridad más alta.

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


Verdadero, no se pueden aplicar reglas con menor prioridad sobre esta regla, cuando esta regla evalúa a verdadero. Solo se aplica para Excel 2007;

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtiene o establece el estilo de los rangos de celdas con formato condicional.

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


El valor de texto en una regla de formato condicional "text contains". Válido solo para type = containsText, notContainsText, beginsWith y endsWith. El valor predeterminado es null.

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


El período de tiempo aplicable en una regla de formato condicional "date occurrin". Válido solo para type = timePeriod. El valor predeterminado es TimePeriodType.Today.

Ver [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


Obtén la instancia "Top10" del formato condicional. La regla de la instancia predeterminada resalta las celdas cuyos valores se encuentran en el rango superior del 10%. Válido solo para type = Top10.

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


Obtiene si el tipo de formato condicional.

Ver [FormatConditionType](../../com.aspose.cells/formatconditiontype).

**Returns:**
int
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




### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Establece el valor o expresión asociado al formato condicional.

**Remarks**

Por favor, añada todas las áreas antes de establecer la fórmula. Para establecer la fórmula de esta condición, si el valor de entrada comienza con '=', se tomará como fórmula. De lo contrario se tomará como valor simple (texto, número, bool). Para valores de texto que comienzan con '=', el usuario puede ingresarlos como fórmula en el formato: "=\\\"=...\\\"".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Establece el valor o expresión asociado a esta condición de formato.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | El valor o expresión asociado con esta condición de formato. Si el valor de entrada comienza con '=', entonces se tomará como fórmula. De lo contrario se tomará como valor simple (texto, número, booleano). Para un valor de texto que comienza con '=', el usuario puede ingresarlo como fórmula en el formato: "=\\"=...\\"". |
| isR1C1 | boolean | Si la fórmula es una fórmula R1C1. |
| isLocal | boolean | Si la fórmula está formateada según la configuración regional. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Establece el valor o expresión asociado al formato condicional.

**Remarks**

Por favor, añada todas las áreas antes de establecer la fórmula. Para establecer la fórmula de esta condición, si el valor de entrada comienza con '=', se tomará como fórmula. De lo contrario se tomará como valor simple (texto, número, bool). Para valores de texto que comienzan con '=', el usuario puede ingresarlos como fórmula en el formato: "=\\\"=...\\\"".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Establece el valor o expresión asociado a esta condición de formato.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | El valor o expresión asociado con esta condición de formato. Si el valor de entrada comienza con '=', entonces se tomará como fórmula. De lo contrario se tomará como valor simple (texto, número, booleano). Para un valor de texto que comienza con '=', el usuario puede ingresarlo como fórmula en el formato: "=\\"=...\\"". |
| isR1C1 | boolean | Si la fórmula es una fórmula R1C1. |
| isLocal | boolean | Si la fórmula está formateada según la configuración regional. |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


Establece el valor o expresión asociado a esta condición de formato.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula1 | java.lang.String | El valor o expresión asociado con esta condición de formato. Si el valor de entrada comienza con '=', entonces se tomará como fórmula. De lo contrario se tomará como valor simple (texto, número, booleano). Para un valor de texto que comienza con '=', el usuario puede ingresarlo como fórmula en el formato: "=\\"=...\\"". |
| formula2 | java.lang.String | El valor o expresión asociado con esta condición de formato. El formato de entrada es el mismo que formula1 |
| isR1C1 | boolean | Si la fórmula es una fórmula R1C1. |
| isLocal | boolean | Si la fórmula está formateada según la configuración regional. |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Establece el tipo de operador del formato condicional.

Ver [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


La prioridad de esta regla de formato condicional. Este valor se usa para determinar qué formato debe evaluarse y renderizarse. Los valores numéricos más bajos tienen mayor prioridad que los valores numéricos más altos, donde '1' es la prioridad más alta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


Verdadero, no se pueden aplicar reglas con menor prioridad sobre esta regla, cuando esta regla evalúa a verdadero. Solo se aplica para Excel 2007;

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Obtiene o establece el estilo de los rangos de celdas con formato condicional.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


El valor de texto en una regla de formato condicional "text contains". Válido solo para type = containsText, notContainsText, beginsWith y endsWith. El valor predeterminado es null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


El período de tiempo aplicable en una regla de formato condicional "date occurrin". Válido solo para type = timePeriod. El valor predeterminado es TimePeriodType.Today.

Ver [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Establece si el tipo de formato condicional.

Ver [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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

