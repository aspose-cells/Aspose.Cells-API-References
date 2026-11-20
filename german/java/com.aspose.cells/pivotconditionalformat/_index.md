---
title: "PivotConditionalFormat"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt das bedingte Format der Pivot-Tabelle dar."
type: docs
url: /de/java/com.aspose.cells/pivotconditionalformat/
---

**Inheritance:**
java.lang.Object
```
public class PivotConditionalFormat
```

Stellt das bedingte Format der Pivot-Tabelle dar.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addCellArea(CellArea ca)](#addCellArea-com.aspose.cells.CellArea-) | Fügt einen Bereich basierend auf der Pivot-Tabellen-Ansicht hinzu. |
| [addFieldArea(int axisType, PivotField field)](#addFieldArea-int-com.aspose.cells.PivotField-) | Fügt einen Bereich des Pivot-Feldes hinzu. |
| [addFieldArea(int axisType, String fieldName)](#addFieldArea-int-java.lang.String-) | Fügt einen Bereich des Pivot-Feldes hinzu. |
| [applyTo(int row, int column, int scope)](#applyTo-int-int-int-) | Wendet das bedingte Format auf einen Bereich an, der sich im Datenbereich befinden muss. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellAreas()](#getCellAreas--) | Liefert alle Zellbereiche, auf die dieses bedingte Format angewendet wird. |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Liefert Bedingungen für das bedingte Format der Pivot-Tabelle . |
| [getPivotAreas()](#getPivotAreas--) | Liefert alle Pivot-Bereiche. |
| [getRuleType()](#getRuleType--) | Liefert den Regeltyp für das bedingte Format der Pivot-Tabelle . |
| [getScopeType()](#getScopeType--) | Ermittelt den Gültigkeitsbereichstyp für das Pivot-Tabellen-Bedingte Format. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRuleType(int value)](#setRuleType-int-) | Legt den Regeltyp für das Pivot-Tabellen-Bedingte Format fest. |
| [setScopeType(int value)](#setScopeType-int-) | Legt den Gültigkeitsbereichstyp für das Pivot-Tabellen-Bedingte Format fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCellArea(CellArea ca) {#addCellArea-com.aspose.cells.CellArea-}
```
public void addCellArea(CellArea ca)
```


Fügt einen Bereich basierend auf der Pivot-Tabellen-Ansicht hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Zellbereich. |

### addFieldArea(int axisType, PivotField field) {#addFieldArea-int-com.aspose.cells.PivotField-}
```
public void addFieldArea(int axisType, PivotField field)
```


Fügt einen Bereich des Pivot-Feldes hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Regionstyp. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Das Pivot-Feld. |

### addFieldArea(int axisType, String fieldName) {#addFieldArea-int-java.lang.String-}
```
public void addFieldArea(int axisType, String fieldName)
```


Fügt einen Bereich des Pivot-Feldes hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Regionstyp. |
| fieldName | java.lang.String | Der Name des Pivot-Feldes. |

### applyTo(int row, int column, int scope) {#applyTo-int-int-int-}
```
public void applyTo(int row, int column, int scope)
```


Wendet das bedingte Format auf einen Bereich an, der sich im Datenbereich befinden muss.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Die ausgewählte Zeile. |
| Spalte | int | Die ausgewählte Spalte. |
| scope | int | [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype). Der Gültigkeitsbereich |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Liefert alle Zellbereiche, auf die dieses bedingte Format angewendet wird.

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


Liefert Bedingungen für das bedingte Format der Pivot-Tabelle .

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getPivotAreas() {#getPivotAreas--}
```
public PivotAreaCollection getPivotAreas()
```


Liefert alle Pivot-Bereiche.

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Liefert den Regeltyp für das bedingte Format der Pivot-Tabelle .

Siehe [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Ermittelt den Gültigkeitsbereichstyp für das Pivot-Tabellen-Bedingte Format.

Siehe [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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


Legt den Regeltyp für das Pivot-Tabellen-Bedingte Format fest.

Siehe [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Legt den Gültigkeitsbereichstyp für das Pivot-Tabellen-Bedingte Format fest.

Siehe [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

