---
title: "FormatConditionCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar villkorsformatering."
type: docs
url: /sv/java/com.aspose.cells/formatconditioncollection/
---

**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```

Representerar villkorsstyrd formatering. FormatConditions kan innehålla upp till tre villkorsformat.

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet.
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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | Lägger till ett formateringsvillkor och påverkad cellområde till FormatConditions. FormatConditions kan innehålla upp till tre villkorsformat. |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Lägger till ett villkorligt formaterat cellområde. |
| [addCondition(int type)](#addCondition-int-) | Lägg till ett formatvillkor. |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | Lägger till ett formateringsvillkor. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar formateringsvillkoret efter index. |
| [getCellArea(int index)](#getCellArea-int-) | Hämtar det villkorligt formaterade cellområdet efter index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet villkor. |
| [getRangeCount()](#getRangeCount--) | Hämtar antalet villkorligt formaterade områden. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | Tar bort det villkorligt formaterade cellområdet efter index. |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | Ta bort villkorlig formatering i området. |
| [removeCondition(int index)](#removeCondition-int-) | Tar bort formateringsvillkoret efter index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```


Lägger till ett formateringsvillkor och påverkad cellområde till FormatConditions. FormatConditions kan innehålla upp till tre villkorsformat. Referenser till andra blad är inte tillåtna i formlerna för villkorlig formatering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Villkorligt formaterat cellområde. |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Typ av villkorlig formatering. Det kan vara någon av medlemmarna i FormatConditionType. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Jämförelseoperator. Det kan vara någon av medlemmarna i OperatorType. |
| formula1 | java.lang.String | Värdet eller uttrycket som är associerat med villkorlig formatering. |
| formula2 | java.lang.String | Värdet eller uttrycket som är associerat med villkorlig formatering |

**Returns:**
int[] - [0]:Formateringsvillkorsobjektets index;[1] Påverkad cellområdes index.
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```


Lägger till ett villkorligt formaterat cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Villkorligt formaterat cellområde. |

**Returns:**
int - Villkorligt formaterat cellområdes index.
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```


Lägg till ett formatvillkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Formatvillkorstyp. |

**Returns:**
int - Index för formateringsvillkorsobjekt;
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```


Lägger till ett formateringsvillkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Typen av formatvillkor. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Operatorns typ |
| formula1 | java.lang.String | Värdet eller uttrycket som är associerat med villkorsformatering. Om inmatningsvärdet börjar med '=', kommer det att behandlas som en formel. Annars behandlas det som ett vanligt värde (text, nummer, bool). För textvärde som börjar med '=', kan användaren ange det som formel i formatet: "=\\"=...\\"". |
| formula2 | java.lang.String | Värdet eller uttrycket som är associerat med villkorsformatering. Inmatningsformatet är samma som formula1. |

**Returns:**
int - Index för formateringsvillkorsobjekt;
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
### get(int index) {#get-int-}
```
public FormatCondition get(int index)
```


Hämtar formateringsvillkoret efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexet för formatvillkoret som ska returneras. |

**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```


Hämtar det villkorligt formaterade cellområdet efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexet för det villkorligt formaterade cellområdet. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Hämtar antalet villkor.

**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Hämtar antalet villkorligt formaterade områden.

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




### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```


Tar bort det villkorligt formaterade cellområdet efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet för det villkorligt formaterade cellområdet som ska tas bort. |

### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


Ta bort villkorlig formatering i området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | StartRow för området. |
| startColumn | int | StartColumn för området. |
| totalRows | int | Antalet rader i intervallet. |
| totalColumns | int | Antalet kolumner i intervallet. |

**Returns:**
boolean - Returnerar TRUE, denna FormatCondtionCollection bör tas bort.
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```


Tar bort formateringsvillkoret efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet för formatvillkoret som ska tas bort. |

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

