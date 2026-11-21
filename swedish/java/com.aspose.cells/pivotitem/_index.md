---
title: "PivotItem"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett objekt i en PivotField-rapport."
type: docs
url: /sv/java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
```

Representerar ett objekt i en PivotField-rapport.

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
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ALL_PAGE_ITEMS_INDEX](#ALL-PAGE-ITEMS-INDEX) | Sentinel-index för att välja alla sidobjekt (0x7FFD, inte ett giltigt index) |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | Hämtar datum/tidsvärdet för pivot‑elementet. Om värdet är null returneras DateTime.MinValue. |
| [getDoubleValue()](#getDoubleValue--) | Hämtar dubbelvärdet för pivot‑elementet. Om värdet är null eller inte ett tal returneras 0. |
| [getFormula()](#getFormula--) | Hämtar formeln för detta beräknade element. |
| [getIndex()](#getIndex--) | Hämtar indexet för pivotelementet i cachefältet. |
| [getName()](#getName--) | Hämtar namnet på pivotelementet. |
| [getPosition()](#getPosition--) | Anger indexet för detta element i alla PivotItems i fältet. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | Anger positionsindexet i PivotItems under samma föräldranod. |
| [getStringValue()](#getStringValue--) | Hämtar strängvärdet för pivotelementet. Om värdet är null returneras "". |
| [getValue()](#getValue--) | Hämtar värdet för pivotelementet |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | Ställer in om pivotelementet är dolt. |
| [isCalculatedItem()](#isCalculatedItem--) | Indikerar om detta pivotelement är ett beräknat formelobjekt. |
| [isDetailHidden()](#isDetailHidden--) | Hämtar om detaljen för detta pivotelement är dold. |
| [isFormula()](#isFormula--) | Indikerar om detta pivotelement är ett beräknat formelobjekt. |
| [isHidden()](#isHidden--) | Hämtar om pivotelementet är dolt. |
| [isHideDetail()](#isHideDetail--) | Hämtar om pivotelementet döljer detaljen. |
| [isMissing()](#isMissing--) | Indikerar om elementet har tagits bort från datakällan. |
| [move(int offset)](#move-int-) | Flyttar elementet upp eller ner i pivåfältet |
| [move(int offset, boolean isSameParent)](#move-int-boolean-) | Flyttar elementet upp eller ner |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | Ställer in om detaljen för detta pivotelement är dold. |
| [setFormula(boolean value)](#setFormula-boolean-) | Indikerar om detta pivotelement är ett beräknat formelobjekt. |
| [setHidden(boolean value)](#setHidden-boolean-) | Ställer in om pivotelementet är dolt. |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | Ställer in om pivotelementet döljer detaljen. |
| [setIndex(int value)](#setIndex-int-) | Hämtar indexet för pivotelementet i cachefältet. |
| [setName(String value)](#setName-java.lang.String-) | Hämtar namnet på pivotelementet. |
| [setPosition(int value)](#setPosition-int-) | Anger indexet för detta element i alla PivotItems i fältet. |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | Anger positionsindexet i PivotItems under samma föräldranod. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL_PAGE_ITEMS_INDEX {#ALL-PAGE-ITEMS-INDEX}
```
public static final short ALL_PAGE_ITEMS_INDEX
```


Sentinel-index för att välja alla sidobjekt (0x7FFD, inte ett giltigt index)

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
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Hämtar datum/tidsvärdet för pivot‑elementet. Om värdet är null returneras DateTime.MinValue.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Hämtar dubbelvärdet för pivot‑elementet. Om värdet är null eller inte ett tal returneras 0.

**Returns:**
double
### getFormula() {#getFormula--}
```
public String getFormula()
```


Hämtar formeln för detta beräknade element. Fungerar endast när detta element är ett beräknat element.

**Returns:**
java.lang.String -
### getIndex() {#getIndex--}
```
public int getIndex()
```


Hämtar indexet för pivotelementet i cachefältet.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotItem.Position‑egenskapen. Denna metod kommer att tas bort 6 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på pivotelementet.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Anger indexet för detta element i alla PivotItems i fältet.

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


Anger positionsindexet i PivotItems under samma föräldranod.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotTable.MoveItem(PivotFieldType, string[],bool,int)-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Hämtar strängvärdet för pivotelementet. Om värdet är null returneras "".

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Hämtar värdet för pivotelementet

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


Ställer in om pivotelementet är dolt.

**Remarks**

OBS: Detta medlem är nu föråldrad. Använd istället Aspose.Cells.Pivot.PivotItem.IsHidden‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med JANUARI 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


Indikerar om detta pivotelement är ett beräknat formelobjekt.

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


Hämtar om detaljen för detta pivotelement är dold.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Indikerar om detta pivotelement är ett beräknat formelobjekt.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotItem.IsCalculatedItem‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Hämtar om pivotelementet är dolt.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


Hämtar om pivotelementet döljer detaljen.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotItem.IsDetailHidden‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


Indikerar om elementet har tagits bort från datakällan.

**Remarks**

Sant betyder att detta värde har tagits bort från datakällan.

**Returns:**
boolean
### move(int offset) {#move-int-}
```
public void move(int offset)
```


Flyttar elementet upp eller ner i pivåfältet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| förskjutning | int | Antalet steg för att flytta upp eller ner. Flytta elementet upp om detta är mindre än noll; flytta elementet ner om detta är större än noll. |

### move(int offset, boolean isSameParent) {#move-int-boolean-}
```
public void move(int offset, boolean isSameParent)
```


Flyttar elementet upp eller ner

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotTable.MoveItem(PivotFieldType, string[],bool,int) eller PivotItem.Move(int)-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| förskjutning | int | Antalet steg för att flytta upp eller ner. Flytta elementet upp om detta är mindre än noll; flytta elementet ner om detta är större än noll. |
| isSameParent | boolean | Anger om flyttoperationen är i samma föräldranod eller inte |

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


Ställer in om detaljen för detta pivotelement är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


Indikerar om detta pivotelement är ett beräknat formelobjekt.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotItem.IsCalculatedItem‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Ställer in om pivotelementet är dolt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


Ställer in om pivotelementet döljer detaljen.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotItem.IsDetailHidden‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


Hämtar indexet för pivotelementet i cachefältet.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotItem.Position‑egenskapen. Denna metod kommer att tas bort 6 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Hämtar namnet på pivotelementet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Anger indexet för detta element i alla PivotItems i fältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


Anger positionsindexet i PivotItems under samma föräldranod.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotTable.MoveItem(PivotFieldType, string[],bool,int)-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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

