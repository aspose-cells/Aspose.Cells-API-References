---
title: "Top10"
second_title: "Aspose.Cells för Java API-referens"
description: "Beskriv Top10-villkorsformateringsregeln."
type: docs
url: /sv/java/com.aspose.cells/top10/
---

**Inheritance:**
java.lang.Object
```
public class Top10
```

Beskriv Top10-regeln för villkorsstyrd formatering. Denna regel markerar celler vars värden faller inom de översta N eller nedersta N intervallen, enligt specifikationen.

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
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [Top10()](#Top10--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | Hämtar värdet på "n" i en "top/bottom n"-regel för villkorsstyrd formatering. |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | Hämtar om en "top/bottom n"-regel är en "bottom n"-regel. |
| [isPercent()](#isPercent--) | Hämtar om en "top/bottom n"-regel är en "top/bottom n percent"-regel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | Ställer in om en "top/bottom n"-regel är en "bottom n"-regel. |
| [setPercent(boolean value)](#setPercent-boolean-) | Ställer in om en "top/bottom n"-regel är en "top/bottom n percent"-regel. |
| [setRank(int value)](#setRank-int-) | Ställer in värdet på "n" i en "top/bottom n"-regel för villkorsstyrd formatering. |
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
| Parameter | Typ | Beskrivning |
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


Hämtar värdet på "n" i en "top/bottom n"-regel för villkorsstyrd formatering. Om IsPercent är sant måste värdet ligga mellan 0 och 100. Annars måste det ligga mellan 0 och 1000. Standardvärdet är 10.

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


Hämtar om en "top/bottom n"-regel är en "bottom n"-regel. Standardvärdet är falskt.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Hämtar om en "top/bottom n"-regel är en "top/bottom n percent"-regel. Standardvärdet är falskt.

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


Ställer in om en "top/bottom n"-regel är en "bottom n"-regel. Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```


Anger om en "top/bottom n"-regel är en "top/bottom n percent"-regel. Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```


Anger värdet på "n" i en "top/bottom n"-villkorsformateringsregel. Om IsPercent är true måste värdet ligga mellan 0 och 100. Annars måste det ligga mellan 0 och 1000. Standardvärdet är 10.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

