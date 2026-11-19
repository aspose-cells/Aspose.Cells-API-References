---
title: "PivotConditionalFormat"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le format conditionnel du tableau croisé dynamique."
type: docs
url: /fr/java/com.aspose.cells/pivotconditionalformat/
---

**Inheritance:**
java.lang.Object
```
public class PivotConditionalFormat
```

Représente le format conditionnel du tableau croisé dynamique.

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
## Méthodes

| Méthode | Description |
| --- | --- |
| [addCellArea(CellArea ca)](#addCellArea-com.aspose.cells.CellArea-) | Ajoute une zone basée sur la vue du tableau croisé dynamique. |
| [addFieldArea(int axisType, PivotField field)](#addFieldArea-int-com.aspose.cells.PivotField-) | Ajoute une zone du champ de tableau croisé dynamique. |
| [addFieldArea(int axisType, String fieldName)](#addFieldArea-int-java.lang.String-) | Ajoute une zone du champ de tableau croisé dynamique. |
| [applyTo(int row, int column, int scope)](#applyTo-int-int-int-) | Applique le format conditionnel à la plage qui doit se trouver dans la région de données. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellAreas()](#getCellAreas--) | Obtient toutes les zones de cellules auxquelles ce format conditionnel s'applique. |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Obtient les conditions du format conditionnel du tableau croisé dynamique. |
| [getPivotAreas()](#getPivotAreas--) | Obtient toutes les zones de tableau croisé dynamique. |
| [getRuleType()](#getRuleType--) | Obtient le type de règle du format conditionnel du tableau croisé dynamique. |
| [getScopeType()](#getScopeType--) | Obtient le type de portée du format conditionnel du tableau croisé dynamique. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRuleType(int value)](#setRuleType-int-) | Définit le type de règle du format conditionnel du tableau croisé dynamique. |
| [setScopeType(int value)](#setScopeType-int-) | Définit le type de portée du format conditionnel du tableau croisé dynamique. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCellArea(CellArea ca) {#addCellArea-com.aspose.cells.CellArea-}
```
public void addCellArea(CellArea ca)
```


Ajoute une zone basée sur la vue du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La zone de cellule. |

### addFieldArea(int axisType, PivotField field) {#addFieldArea-int-com.aspose.cells.PivotField-}
```
public void addFieldArea(int axisType, PivotField field)
```


Ajoute une zone du champ de tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Le type de région. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Le champ du tableau croisé dynamique. |

### addFieldArea(int axisType, String fieldName) {#addFieldArea-int-java.lang.String-}
```
public void addFieldArea(int axisType, String fieldName)
```


Ajoute une zone du champ de tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Le type de région. |
| fieldName | java.lang.String | Le nom du champ du tableau croisé dynamique. |

### applyTo(int row, int column, int scope) {#applyTo-int-int-int-}
```
public void applyTo(int row, int column, int scope)
```


Applique le format conditionnel à la plage qui doit se trouver dans la région de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | La ligne sélectionnée. |
| colonne | int | La colonne sélectionnée. |
| scope | int | [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype). La portée |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Obtient toutes les zones de cellules auxquelles ce format conditionnel s'applique.

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


Obtient les conditions du format conditionnel du tableau croisé dynamique.

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getPivotAreas() {#getPivotAreas--}
```
public PivotAreaCollection getPivotAreas()
```


Obtient toutes les zones de tableau croisé dynamique.

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Obtient le type de règle du format conditionnel du tableau croisé dynamique.

Voir [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Obtient le type de portée du format conditionnel du tableau croisé dynamique.

Voir [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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


Définit le type de règle du format conditionnel du tableau croisé dynamique.

Voir [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Définit le type de portée du format conditionnel du tableau croisé dynamique.

Voir [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

