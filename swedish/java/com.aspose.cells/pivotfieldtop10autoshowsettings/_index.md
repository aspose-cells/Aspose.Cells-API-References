---
title: "PivotFieldTop10AutoShowSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar Top 10 AutoShow-inställningarna för ett pivottfält."
type: docs
url: /sv/java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

Representerar Top 10 AutoShow-inställningarna för ett pivottfält.

**Remarks**

I xls: Implementering av top 10-filter i Xls via Top 10 AutoShow. I ooxml-filer: Det underliggande ooxml-filformatet stöder Top10 AutoShow, men Excel 2007 och senare användargränssnitt ger endast åtkomst via Top10-filter. Om XLS-kompatibilitet inte krävs rekommenderas att använda Top10-filter istället.

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
 
         //Show top 2 items by row field label.
         rowField.top10AutoShow(true, true, 2, -1);
 
         PivotFieldTop10AutoShowSettings sortSetting = rowField.getTop10AutoShowSettings();
         System.out.println(sortSetting.isAutoShow());
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | Representerar antalet översta eller nedersta objekt som automatiskt visas i det angivna PivotTable-fältet. |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | Anger indexet för datafältet för AutoShow-rangordning. |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | Indikerar om ett "Top 10 AutoShow"-filter har tillämpats på detta fält. |
| [isTop()](#isTop--) | Indikerar om det angivna PivotTable-fältet automatiskt visas i stigande ordning. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indikerar om ett "Top 10 AutoShow"-filter har tillämpats på detta fält. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Representerar antalet översta eller nedersta objekt som automatiskt visas i det angivna PivotTable-fältet. |
| [setRankBy(int value)](#setRankBy-int-) | Anger indexet för datafältet för AutoShow-rangordning. |
| [setTop(boolean value)](#setTop-boolean-) | Indikerar om det angivna PivotTable-fältet automatiskt visas i stigande ordning. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Representerar antalet översta eller nedersta objekt som automatiskt visas i det angivna PivotTable-fältet.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRankBy() {#getRankBy--}
```
public int getRankBy()
```


Anger indexet för datafältet för AutoShow-rangordning. Representerar auto‑show‑fältets index. -1 betyder PivotField själv. Det bör vara indexet för datafälten.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indikerar om ett "Top 10 AutoShow"-filter har tillämpats på detta fält.

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


Indikerar om det angivna PivotTable-fältet automatiskt visas i stigande ordning.

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




### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indikerar om ett "Top 10 AutoShow"-filter har tillämpats på detta fält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Representerar antalet översta eller nedersta objekt som automatiskt visas i det angivna PivotTable-fältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


Anger indexet för datafältet för AutoShow-rangordning. Representerar auto‑show‑fältets index. -1 betyder PivotField själv. Det bör vara indexet för datafälten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


Indikerar om det angivna PivotTable-fältet automatiskt visas i stigande ordning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

