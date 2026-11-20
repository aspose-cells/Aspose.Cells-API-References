---
title: "PivotShowValuesSetting"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Einstellungen zum Anzeigen von Werten dar, wenn die ShowDataAs‑Berechnung verwendet wird."
type: docs
url: /de/java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

Stellt die Einstellungen zum Anzeigen von Werten dar, wenn die ShowDataAs‑Berechnung verwendet wird.

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
 
         PivotField dataField = pivot.getDataFields().get(0);
         // Display value as percentage of the grand total
         dataField.showValuesAs(PivotShowValuesAsType.PERCENTAGE_OF_TOTAL, 0, PivotShowValuesSetting.NEXT_PIVOT_ITEM);
         // Get the display calculation setting of data field
         PivotShowValuesSetting settings = dataField.getShowValuesSetting();
         System.out.println(settings.getShowValuesAs());
 
          pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Felder

| Feld | Beschreibung |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | Spezialer Basis-Element-Index: Verwenden Sie das nachfolgende Pivot-Element. |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | Spezialer Basis-Element-Index: Verwenden Sie das vorherige Pivot-Element. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Stellt das Basisfeld für eine ShowDataAs-Berechnung dar, wenn die ShowDataAs-Berechnung verwendet wird. |
| [getBaseFieldName()](#getBaseFieldName--) | Liefert die Beschriftung des Pivot-Basisfelds. |
| [getBaseItemCaption()](#getBaseItemCaption--) | Liefert die Beschriftung des Pivot-Elements im Basisfeld. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Stellt den benutzerdefinierten Index des Pivot-Elements im Basisfeld dar, wenn die ShowDataAs-Berechnung verwendet wird. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | Stellt den Typ des Basis-Pivot-Elements im Basisfeld dar, wenn die ShowDataAs-Berechnung verwendet wird. |
| [getCalculationType()](#getCalculationType--) | Stellt dar, wie Werte eines Datenfelds im Pivot-Bericht angezeigt werden. |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | Liefert, wie Werte eines Datenfelds im Pivot-Bericht angezeigt werden. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Stellt das Basisfeld für eine ShowDataAs-Berechnung dar, wenn die ShowDataAs-Berechnung verwendet wird. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Stellt den benutzerdefinierten Index des Pivot-Elements im Basisfeld dar, wenn die ShowDataAs-Berechnung verwendet wird. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | Stellt den Typ des Basis-Pivot-Elements im Basisfeld dar, wenn die ShowDataAs-Berechnung verwendet wird. |
| [setCalculationType(int value)](#setCalculationType-int-) | Stellt dar, wie Werte eines Datenfelds im Pivot-Bericht angezeigt werden. |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | Legt fest, wie Werte eines Datenfelds im Pivot-Bericht angezeigt werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


Spezialer Basis-Element-Index: Verwenden Sie das nachfolgende Pivot-Element. Gültig für "Show Values As"-Berechnungen; wirksam ab Excel 2010.

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


Spezialer Basis-Element-Index: Verwenden Sie das vorherige Pivot-Element. Gültig für "Show Values As"-Berechnungen; wirksam ab Excel 2010.

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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


Stellt das Basisfeld für eine ShowDataAs-Berechnung dar, wenn die ShowDataAs-Berechnung verwendet wird.

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


Liefert die Beschriftung des Pivot-Basisfelds.

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


Liefert die Beschriftung des Pivot-Elements im Basisfeld.

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


Stellt den benutzerdefinierten Index des Pivot-Elements im Basisfeld dar, wenn die ShowDataAs-Berechnung verwendet wird.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


Stellt den Typ des Basis-Pivot-Elements im Basisfeld dar, wenn die ShowDataAs-Berechnung verwendet wird. Da PivotItemPosition.Custom nur lesbar ist, setzen Sie bei Bedarf PivotItemPosition.Custom, bitte das Attribut PivotField.BaseItemIndex.

Siehe [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotShowValuesSetting.BaseItem. Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


Stellt dar, wie Werte eines Datenfelds im Pivot-Bericht angezeigt werden.

Siehe [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotShowValuesSetting.ShowValuesAs. Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getShowValuesAs() {#getShowValuesAs--}
```
public int getShowValuesAs()
```


Liefert, wie Werte eines Datenfelds im Pivot-Bericht angezeigt werden.

Siehe [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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




### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


Stellt das Basisfeld für eine ShowDataAs-Berechnung dar, wenn die ShowDataAs-Berechnung verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Stellt den benutzerdefinierten Index des Pivot-Elements im Basisfeld dar, wenn die ShowDataAs-Berechnung verwendet wird.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


Stellt den Typ des Basis-Pivot-Elements im Basisfeld dar, wenn die ShowDataAs-Berechnung verwendet wird. Da PivotItemPosition.Custom nur lesbar ist, setzen Sie bei Bedarf PivotItemPosition.Custom, bitte das Attribut PivotField.BaseItemIndex.

Siehe [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotShowValuesSetting.BaseItem. Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


Stellt dar, wie Werte eines Datenfelds im Pivot-Bericht angezeigt werden.

Siehe [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotShowValuesSetting.ShowValuesAs. Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


Legt fest, wie Werte eines Datenfelds im Pivot-Bericht angezeigt werden.

Siehe [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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

