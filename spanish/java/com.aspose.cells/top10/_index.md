---
title: "Top10"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Describe la regla de formato condicional Top10."
type: docs
url: /es/java/com.aspose.cells/top10/
---

**Inheritance:**
java.lang.Object
```
public class Top10
```

Describe la regla de formato condicional Top10. Esta regla de formato condicional resalta celdas cuyos valores se encuentran en el rango superior N o inferior N, según se especifique.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = CellArea.createCellArea(0, 0, 10, 10);
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.TOP_10, OperatorType.NONE, null, null);   
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         Top10 top10 = fc.getTop10();
         //Set the Top N 
         top10.setRank(5);  
         //Saving the Excel file
         workbook.save("output.xls");
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Top10()](#Top10--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | Obtiene el valor de "n" en una regla de formato condicional "top/bottom n". |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | Obtiene si una regla "top/bottom n" es una regla "bottom n". |
| [isPercent()](#isPercent--) | Obtiene si una regla "top/bottom n" es una regla "top/bottom n percent". |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | Establece si una regla "top/bottom n" es una regla "bottom n". |
| [setPercent(boolean value)](#setPercent-boolean-) | Establece si una regla "top/bottom n" es una regla "top/bottom n percent". |
| [setRank(int value)](#setRank-int-) | Establece el valor de "n" en una regla de formato condicional "top/bottom n". |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Top10() {#Top10--}
```
public Top10()
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
### getRank() {#getRank--}
```
public int getRank()
```


Obtiene el valor de "n" en una regla de formato condicional "top/bottom n". Si IsPercent es verdadero, el valor debe estar entre 0 y 100. De lo contrario debe estar entre 0 y 1000. El valor predeterminado es 10.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Obtiene si una regla "top/bottom n" es una regla "bottom n". El valor predeterminado es false.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Obtiene si una regla "top/bottom n" es una regla "top/bottom n percent". El valor predeterminado es false.

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




### setBottom(boolean value) {#setBottom-boolean-}
```
public void setBottom(boolean value)
```


Establece si una regla "top/bottom n" es una regla "bottom n". El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```


Establece si una regla "top/bottom n" es una regla "top/bottom n percent". El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```


Establece el valor de "n" en una regla de formato condicional "top/bottom n". Si IsPercent es verdadero, el valor debe estar entre 0 y 100. De lo contrario debe estar entre 0 y 1000. El valor predeterminado es 10.

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

