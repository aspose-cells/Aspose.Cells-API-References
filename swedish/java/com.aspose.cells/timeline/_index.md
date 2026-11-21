---
title: "Tidslinje"
second_title: "Aspose.Cells för Java API-referens"
description: "Sammanfattande beskrivning av tidslinjevyn På grund av att MS Excel 2003 inte stöder tidslinje"
type: docs
url: /sv/java/com.aspose.cells/timeline/
---

**Inheritance:**
java.lang.Object
```
public class Timeline
```

Sammanfattande beskrivning av tidslinjevy på grund av MS Excel stöder inte Excel 2003 tidslinjer.

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
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
         //Add time line based on date field.
         int index = sheet.getTimelines().add(pivot, "E1","date");
         Timeline timeline = sheet.getTimelines().get(index);
 
         //do your business
         book.save("out.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | Hämtar rubriken för denna tidslinje. |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | Den aktuella tidsnivån för tidslinjen. |
| [getHeightPixel()](#getHeightPixel--) | Returnerar eller anger höjden på den angivna tidslinjen, i pixlar. |
| [getLeftPixel()](#getLeftPixel--) | Returnerar eller anger den horisontella förskjutningen för tidslinjeformen från dess vänstra kolumn, i pixlar. |
| [getName()](#getName--) | Returnerar eller anger namnet på den angivna tidslinjen |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--) | Hämtar det valda datum- och tidsintervallet. |
| [getSelectionLevel()](#getSelectionLevel--) | Hämtar tidsnivån som den aktuella markeringen gjordes på för tidslinjen. |
| [getShape()](#getShape--) | Returnerar [TimelineShape](../../com.aspose.cells/timelineshape)-objektet som är associerat med denna tidslinje. |
| [getShowHeader()](#getShowHeader--) | Anger om rubriken för denna tidslinje ska visas. |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | Anger om den horisontella rullningslisten ska visas. |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | Anger om urvalsetiketten ska visas. |
| [getShowTimeLevel()](#getShowTimeLevel--) | Anger om rullgardinsmenyn för tidsnivån ska visas. |
| [getStartDate()](#getStartDate--) | Hämtar startdatumet för tidsintervallens rullningsposition för denna [Timeline](../../com.aspose.cells/timeline). |
| [getTopPixel()](#getTopPixel--) | Returnerar eller anger den vertikala förskjutningen för tidslinjeformen från dess översta rad, i pixlar. |
| [getWidthPixel()](#getWidthPixel--) | Returnerar eller anger bredden på den angivna tidslinjen, i pixlar. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(DateTime start, DateTime end, boolean calculate)](#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-) | Välj objekt mellan datum och tid. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Anger rubriken för denna tidslinje. |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | Den aktuella tidsnivån för tidslinjen. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Returnerar eller anger höjden på den angivna tidslinjen, i pixlar. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Returnerar eller anger den horisontella förskjutningen för tidslinjeformen från dess vänstra kolumn, i pixlar. |
| [setName(String value)](#setName-java.lang.String-) | Returnerar eller anger namnet på den angivna tidslinjen |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | Anger tidsnivån som den aktuella markeringen gjordes på för tidslinjen. |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | Anger om rubriken för denna tidslinje ska visas. |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | Anger om den horisontella rullningslisten ska visas. |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | Anger om urvalsetiketten ska visas. |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | Anger om rullgardinsmenyn för tidsnivån ska visas. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Anger startdatumet för tidsintervallens rullningsposition för denna [Timeline](../../com.aspose.cells/timeline). |
| [setTopPixel(int value)](#setTopPixel-int-) | Returnerar eller anger den vertikala förskjutningen för tidslinjeformen från dess översta rad, i pixlar. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Returnerar eller anger bredden på den angivna tidslinjen, i pixlar. |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


Hämtar rubriken för denna tidslinje.

**Example**

```
         //Set the caption of this Timeline.
         timeline.setCaption("timeline caption test");
```

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


Den aktuella tidsnivån för tidslinjen.

Se [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Returnerar eller anger höjden på den angivna tidslinjen, i pixlar.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.Height. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Returnerar eller anger den horisontella förskjutningen för tidslinjeformen från dess vänstra kolumn, i pixlar.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.Left. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Returnerar eller anger namnet på den angivna tidslinjen

**Example**

```
         //Set the name of the specified Timeline.
         timeline.setName("timeline name test");
```

**Returns:**
java.lang.String
### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}
```
public DateTime[] getSelectedDateTimeRange()
```


Hämtar det valda datum- och tidsintervallet.

**Returns:**
com.aspose.cells.DateTime[] -
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


Hämtar tidsnivån som den aktuella markeringen gjordes på för tidslinjen.

Se [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


Returnerar [TimelineShape](../../com.aspose.cells/timelineshape)-objektet som är associerat med denna tidslinje.

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


Anger om rubriken för denna tidslinje ska visas.

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


Anger om den horisontella rullningslisten ska visas.

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


Anger om urvalsetiketten ska visas.

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


Anger om rullgardinsmenyn för tidsnivån ska visas.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Hämtar startdatumet för tidsintervallens rullningsposition för denna [Timeline](../../com.aspose.cells/timeline).

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Returnerar eller anger den vertikala förskjutningen för tidslinjeformen från dess översta rad, i pixlar.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället Shape.Top-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Returnerar eller anger bredden på den angivna tidslinjen, i pixlar.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället Shape.Width-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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




### select(DateTime start, DateTime end, boolean calculate) {#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-}
```
public void select(DateTime start, DateTime end, boolean calculate)
```


Välj objekt mellan datum och tid.

**Remarks**

[getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--) must be set before calling this method. If this method is called, [getSelectionLevel()](../../com.aspose.cells/timeline\#getSelectionLevel--) will be [getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | Startdatum och tid |
| end | [DateTime](../../com.aspose.cells/datetime) | Slutdatum och tid |
| beräkna | boolean | Anger om relativa pivottabeller ska beräknas |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Anger rubriken för denna tidslinje.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


Den aktuella tidsnivån för tidslinjen.

Se [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Returnerar eller anger höjden på den angivna tidslinjen, i pixlar.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.Height. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


Returnerar eller anger den horisontella förskjutningen för tidslinjeformen från dess vänstra kolumn, i pixlar.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.Left. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Returnerar eller anger namnet på den angivna tidslinjen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


Anger tidsnivån som den aktuella markeringen gjordes på för tidslinjen.

Se [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


Anger om rubriken för denna tidslinje ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


Anger om den horisontella rullningslisten ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


Anger om urvalsetiketten ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


Anger om rullgardinsmenyn för tidsnivån ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Anger startdatumet för tidsintervallens rullningsposition för denna [Timeline](../../com.aspose.cells/timeline).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Returnerar eller anger den vertikala förskjutningen för tidslinjeformen från dess översta rad, i pixlar.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället Shape.Top-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Returnerar eller anger bredden på den angivna tidslinjen, i pixlar.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället Shape.Width-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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

