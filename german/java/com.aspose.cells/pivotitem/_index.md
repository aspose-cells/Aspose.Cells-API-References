---
title: "PivotItem"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt ein Element in einem PivotField‑Bericht dar."
type: docs
url: /de/java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
```

Stellt ein Element in einem PivotField‑Bericht dar.

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
 
          //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Hide the first item
         PivotItem item = rowField.getPivotItems().get(0);          
         item.setHidden(true);
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Felder

| Feld | Beschreibung |
| --- | --- |
| [ALL_PAGE_ITEMS_INDEX](#ALL-PAGE-ITEMS-INDEX) | Sentinel-Index für 'Alle auswählen' von Seitenelementen (0x7FFD, kein gültiger Index) |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | Gibt den Datums-/Uhrzeitwert des Pivot-Elements zurück. Wenn der Wert null ist, wird DateTime.MinValue zurückgegeben. |
| [getDoubleValue()](#getDoubleValue--) | Gibt den Double-Wert des Pivot-Elements zurück. Wenn der Wert null oder keine Zahl ist, wird 0 zurückgegeben. |
| [getFormula()](#getFormula--) | Ruft die Formel dieses berechneten Elements ab. |
| [getIndex()](#getIndex--) | Ruft den Index des Pivot-Elements im Cache-Feld ab. |
| [getName()](#getName--) | Ruft den Namen des Pivot-Elements ab. |
| [getPosition()](#getPosition--) | Gibt den Index dieses Elements in allen PivotItems des Feldes an. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | Gibt den Positionsindex in den PivotItems unter demselben übergeordneten Knoten an. |
| [getStringValue()](#getStringValue--) | Ruft den Zeichenkettenwert des Pivot-Elements ab. Wenn der Wert null ist, wird "" zurückgegeben. |
| [getValue()](#getValue--) | Ruft den Wert des Pivot-Elements ab |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | Legt fest, ob das Pivot-Element ausgeblendet ist. |
| [isCalculatedItem()](#isCalculatedItem--) | Gibt an, ob dieses Pivot-Element ein berechnetes Formelelement ist. |
| [isDetailHidden()](#isDetailHidden--) | Ruft ab, ob das Detail dieses Pivot-Elements ausgeblendet ist. |
| [isFormula()](#isFormula--) | Gibt an, ob dieses Pivot-Element ein berechnetes Formelelement ist. |
| [isHidden()](#isHidden--) | Ruft ab, ob das Pivot-Element ausgeblendet ist. |
| [isHideDetail()](#isHideDetail--) | Ruft ab, ob das Pivot-Element Details ausblendet. |
| [isMissing()](#isMissing--) | Gibt an, ob das Element aus der Datenquelle entfernt wurde. |
| [move(int offset)](#move-int-) | Verschiebt das Element im Pivot-Feld nach oben oder unten |
| [move(int offset, boolean isSameParent)](#move-int-boolean-) | Verschiebt das Element nach oben oder unten |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | Legt fest, ob das Detail dieses Pivot-Elements ausgeblendet ist. |
| [setFormula(boolean value)](#setFormula-boolean-) | Gibt an, ob dieses Pivot-Element ein berechnetes Formelelement ist. |
| [setHidden(boolean value)](#setHidden-boolean-) | Legt fest, ob das Pivot-Element ausgeblendet ist. |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | Legt fest, ob das Pivot-Element Details ausblendet. |
| [setIndex(int value)](#setIndex-int-) | Ruft den Index des Pivot-Elements im Cache-Feld ab. |
| [setName(String value)](#setName-java.lang.String-) | Ruft den Namen des Pivot-Elements ab. |
| [setPosition(int value)](#setPosition-int-) | Gibt den Index dieses Elements in allen PivotItems des Feldes an. |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | Gibt den Positionsindex in den PivotItems unter demselben übergeordneten Knoten an. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL_PAGE_ITEMS_INDEX {#ALL-PAGE-ITEMS-INDEX}
```
public static final short ALL_PAGE_ITEMS_INDEX
```


Sentinel-Index für 'Alle auswählen' von Seitenelementen (0x7FFD, kein gültiger Index)

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Gibt den Datums-/Uhrzeitwert des Pivot-Elements zurück. Wenn der Wert null ist, wird DateTime.MinValue zurückgegeben.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Gibt den Double-Wert des Pivot-Elements zurück. Wenn der Wert null oder keine Zahl ist, wird 0 zurückgegeben.

**Returns:**
double
### getFormula() {#getFormula--}
```
public String getFormula()
```


Ruft die Formel dieses berechneten Elements ab. Funktioniert nur, wenn dieses Element ein berechnetes Element ist.

**Returns:**
java.lang.String -
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ruft den Index des Pivot-Elements im Cache-Feld ab.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die PivotItem.Position-Eigenschaft. Diese Methode wird 6 Monate später, seit August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ruft den Namen des Pivot-Elements ab.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Gibt den Index dieses Elements in allen PivotItems des Feldes an.

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


Gibt den Positionsindex in den PivotItems unter demselben übergeordneten Knoten an.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Stattdessen verwenden Sie bitte die Methode PivotTable.MoveItem(PivotFieldType, string[],bool,int). Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Ruft den Zeichenkettenwert des Pivot-Elements ab. Wenn der Wert null ist, wird "" zurückgegeben.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Ruft den Wert des Pivot-Elements ab

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hide(boolean value) {#hide-boolean-}
```
public void hide(boolean value)
```


Legt fest, ob das Pivot-Element ausgeblendet ist.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft Aspose.Cells.Pivot.PivotItem.IsHidden. Diese Eigenschaft wird 12 Monate später, seit JANUARY 2012, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


Gibt an, ob dieses Pivot-Element ein berechnetes Formelelement ist.

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


Ruft ab, ob das Detail dieses Pivot-Elements ausgeblendet ist.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Gibt an, ob dieses Pivot-Element ein berechnetes Formelelement ist.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotItem.IsCalculatedItem. Diese Eigenschaft wird 12 Monate später, seit November 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Ruft ab, ob das Pivot-Element ausgeblendet ist.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


Ruft ab, ob das Pivot-Element Details ausblendet.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotItem.IsDetailHidden. Diese Eigenschaft wird 12 Monate später, seit November 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


Gibt an, ob das Element aus der Datenquelle entfernt wurde.

**Remarks**

True bedeutet, dass dieser Wert aus der Datenquelle entfernt wurde.

**Returns:**
boolean
### move(int offset) {#move-int-}
```
public void move(int offset)
```


Verschiebt das Element im Pivot-Feld nach oben oder unten

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| offset | int | Die Anzahl der Verschiebungen nach oben oder unten. Verschieben Sie das Element nach oben, wenn dieser Wert kleiner als null ist; verschieben Sie das Element nach unten, wenn dieser Wert größer als null ist. |

### move(int offset, boolean isSameParent) {#move-int-boolean-}
```
public void move(int offset, boolean isSameParent)
```


Verschiebt das Element nach oben oder unten

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen bitte die Methode PivotTable.MoveItem(PivotFieldType, string[],bool,int) oder PivotItem.Move(int). Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| offset | int | Die Anzahl der Verschiebungen nach oben oder unten. Verschieben Sie das Element nach oben, wenn dieser Wert kleiner als null ist; verschieben Sie das Element nach unten, wenn dieser Wert größer als null ist. |
| isSameParent | boolean | Angabe, ob der Verschiebevorgang im selben übergeordneten Knoten erfolgt oder nicht |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDetailHidden(boolean value) {#setDetailHidden-boolean-}
```
public void setDetailHidden(boolean value)
```


Legt fest, ob das Detail dieses Pivot-Elements ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


Gibt an, ob dieses Pivot-Element ein berechnetes Formelelement ist.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotItem.IsCalculatedItem. Diese Eigenschaft wird 12 Monate später, seit November 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Legt fest, ob das Pivot-Element ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


Legt fest, ob das Pivot-Element Details ausblendet.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft PivotItem.IsDetailHidden. Diese Eigenschaft wird 12 Monate später, seit November 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


Ruft den Index des Pivot-Elements im Cache-Feld ab.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die PivotItem.Position-Eigenschaft. Diese Methode wird 6 Monate später, seit August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ruft den Namen des Pivot-Elements ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Gibt den Index dieses Elements in allen PivotItems des Feldes an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


Gibt den Positionsindex in den PivotItems unter demselben übergeordneten Knoten an.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Stattdessen verwenden Sie bitte die Methode PivotTable.MoveItem(PivotFieldType, string[],bool,int). Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

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

