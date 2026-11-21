---
title: "DiscreteGroupItem"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett objekt av anpassat grupperat fält."
type: docs
url: /sv/java/com.aspose.cells/discretegroupitem/
---

**Inheritance:**
java.lang.Object
```
public class DiscreteGroupItem
```

Representerar ett objekt av anpassat grupperat fält.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("product");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("carrot");
         cells.get(3, 0).setValue("potato");
         cells.get(4, 0).setValue("cherry");
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "product");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Group by fruit and vegetable
         DiscreteGroupItem fruit = new DiscreteGroupItem("fruit", new int[] { 0, 3 });
         DiscreteGroupItem vegetable = new DiscreteGroupItem("vegetable", new int[] { 1, 2 });
         PivotFieldGroupOptions groupOptions = new PivotFieldGroupOptions();
         groupOptions.setDiscreteGroupItems(new DiscreteGroupItem[] { fruit, vegetable });
         pivot.getRowFields().get(0).group(groupOptions);
         pivot.calculateData();
 
         //do your business
 
         book.save("DiscreteGroup.xlsx");
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [DiscreteGroupItem(String name, int[] itemIndexes)](#DiscreteGroupItem-java.lang.String-int---) | Konstruktorn för anpassat gruppobjekt för pivottfältet. |
| [DiscreteGroupItem(String name, String[] items)](#DiscreteGroupItem-java.lang.String-java.lang.String---) | Konstruktorn för anpassat gruppobjekt för pivottfältet. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DiscreteGroupItem(String name, int[] itemIndexes) {#DiscreteGroupItem-java.lang.String-int---}
```
public DiscreteGroupItem(String name, int[] itemIndexes)
```


Konstruktorn för anpassat gruppobjekt för pivottfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på gruppobjektet |
| itemIndexes | int[] | Alla index till objekten i baspivottfältet. |

### DiscreteGroupItem(String name, String[] items) {#DiscreteGroupItem-java.lang.String-java.lang.String---}
```
public DiscreteGroupItem(String name, String[] items)
```


Konstruktorn för anpassat gruppobjekt för pivottfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på gruppobjektet |
| items | java.lang.String[] | Rubrikerna för pivotelement som tillhör denna diskreta grupp. |

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

