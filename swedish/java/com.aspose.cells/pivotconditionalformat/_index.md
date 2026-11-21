---
title: "PivotConditionalFormat"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar den villkorliga formateringen av pivottabellen."
type: docs
url: /sv/java/com.aspose.cells/pivotconditionalformat/
---

**Inheritance:**
java.lang.Object
```
public class PivotConditionalFormat
```

Representerar den villkorliga formateringen av pivottabellen.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
 
 
         //do your business
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addCellArea(CellArea ca)](#addCellArea-com.aspose.cells.CellArea-) | Lägger till ett område baserat på pivottabellvyn. |
| [addFieldArea(int axisType, PivotField field)](#addFieldArea-int-com.aspose.cells.PivotField-) | Lägger till ett område av pivottfält. |
| [addFieldArea(int axisType, String fieldName)](#addFieldArea-int-java.lang.String-) | Lägger till ett område av pivottfält. |
| [applyTo(int row, int column, int scope)](#applyTo-int-int-int-) | Tillämpar det villkorliga formatet på ett område som måste ligga i dataregionen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellAreas()](#getCellAreas--) | Hämtar alla cellområden som detta villkorliga format gäller för. |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Hämta villkor för pivottabellens villkorliga format. |
| [getPivotAreas()](#getPivotAreas--) | Hämtar alla pivotområden. |
| [getRuleType()](#getRuleType--) | Hämtar regeltyp för pivottabellens villkorliga format. |
| [getScopeType()](#getScopeType--) | Hämtar omfångstyp för pivottabellens villkorliga format. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRuleType(int value)](#setRuleType-int-) | Anger regeltyp för pivottabellens villkorliga format. |
| [setScopeType(int value)](#setScopeType-int-) | Anger omfångstyp för pivottabellens villkorliga format. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCellArea(CellArea ca) {#addCellArea-com.aspose.cells.CellArea-}
```
public void addCellArea(CellArea ca)
```


Lägger till ett område baserat på pivottabellvyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Cellområdet. |

### addFieldArea(int axisType, PivotField field) {#addFieldArea-int-com.aspose.cells.PivotField-}
```
public void addFieldArea(int axisType, PivotField field)
```


Lägger till ett område av pivottfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Regionstypen. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Pivottfältet. |

### addFieldArea(int axisType, String fieldName) {#addFieldArea-int-java.lang.String-}
```
public void addFieldArea(int axisType, String fieldName)
```


Lägger till ett område av pivottfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Regionstypen. |
| fieldName | java.lang.String | Namnet på pivottfältet. |

### applyTo(int row, int column, int scope) {#applyTo-int-int-int-}
```
public void applyTo(int row, int column, int scope)
```


Tillämpar det villkorliga formatet på ett område som måste ligga i dataregionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Den valda raden. |
| kolumn | int | Den valda kolumnen. |
| scope | int | [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype). Omfattningen |

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
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Hämtar alla cellområden som detta villkorliga format gäller för.

**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Hämta villkor för pivottabellens villkorliga format.

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getPivotAreas() {#getPivotAreas--}
```
public PivotAreaCollection getPivotAreas()
```


Hämtar alla pivotområden.

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Hämtar regeltyp för pivottabellens villkorliga format.

Se [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Hämtar omfångstyp för pivottabellens villkorliga format.

Se [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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




### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Anger regeltyp för pivottabellens villkorliga format.

Se [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Anger omfångstyp för pivottabellens villkorliga format.

Se [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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

