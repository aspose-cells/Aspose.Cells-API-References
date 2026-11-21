---
title: "Slicer"
second_title: "Aspose.Cells för Java API-referens"
description: "sammanfattande beskrivning av Slicer View"
type: docs
url: /sv/java/com.aspose.cells/slicer/
---

**Inheritance:**
java.lang.Object
```
public class Slicer
```

sammanfattande beskrivning av Slicer View

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
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         slicer.unselectItems(new String[] { "grape" });
         //do your business
         book.save("out.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | Lägger till PivotTable-anslutning. |
| [clearFilter()](#clearFilter--) | Ta bort filter |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Returnerar eller anger den beskrivande (alternativa) textsträngen för Slicer-objektet. |
| [getCaption()](#getCaption--) | Returnerar eller anger rubriken för den angivna slicern. |
| [getCaptionVisible()](#getCaptionVisible--) | Returnerar eller anger om rubriken som visar slicer‑rubriken är synlig. |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | Returnerar eller anger bredden på varje kolumn i slicern i enheten punkter. |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | Hämtar bredden på\u807dvarje kolumn i\u807dslicern, i enheten\u807dpixlar.\u807d |
| [getFirstItemIndex()](#getFirstItemIndex--) | Anger det nollbaserade indexet för det första slicer‑objektet. |
| [getHeight()](#getHeight--) | Returnerar eller anger höjden på den angivna slicern, i punkter. |
| [getHeightPixel()](#getHeightPixel--) | Returnerar eller anger höjden på den angivna slicern, i pixlar. |
| [getLeftPixel()](#getLeftPixel--) | Returnerar eller anger den horisontella förskjutningen för slicer‑formen från dess vänstra kolumn, i pixlar. |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | Indikerar om bildförhållandet är låst. |
| [getLockedPosition()](#getLockedPosition--) | Indikerar om den angivna slicern kan flyttas eller storleksändras via användargränssnittet. |
| [getName()](#getName--) | Returnerar eller anger namnet på den angivna slicern |
| [getNumberOfColumns()](#getNumberOfColumns--) | Returnerar eller anger antalet kolumner i slicern. |
| [getParent()](#getParent--) | Returnerar [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--)‑objektet som innehåller denna slicer. |
| [getPlacement()](#getPlacement--) | Representerar hur ritobjektet är fäst vid cellerna under det. |
| [getRowHeight()](#getRowHeight--) | Returnerar eller anger höjden på varje rad i den angivna slicern i enheten punkter. |
| [getRowHeightPixel()](#getRowHeightPixel--) | Returnerar eller anger höjden på varje rad i den angivna slicern, i enheten pixlar. |
| [getShape()](#getShape--) | Returnerar Shape-objektet som är associerat med den angivna slicern. |
| [getShowAllItems()](#getShowAllItems--) | Anger om alla objekt ska visas även om det inte finns någon data eller de har raderats. |
| [getShowCaption()](#getShowCaption--) | Anger om slicer‑rubriken är synlig. |
| [getShowMissing()](#getShowMissing--) | Anger om objekt som har tagits bort från datakällan ska visas. |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--) | Anger om objekt som har tagits bort från datakällan ska visas. |
| [getSlicerCache()](#getSlicerCache--) | Returnerar SlicerCache-objektet som är associerat med slicern. |
| [getSortOrderType()](#getSortOrderType--) | Anger typen av sorteringsobjekt. |
| [getStyleType()](#getStyleType--) | Ange typen av inbyggd slicer‑stil. |
| [getTitle()](#getTitle--) | Anger titeln på det aktuella Slicer‑objektet. |
| [getTopPixel()](#getTopPixel--) | Returnerar eller anger det vertikala offsetet för slicer‑formen från dess översta rad, i pixlar. |
| [getWidth()](#getWidth--) | Returnerar eller anger bredden på den angivna slicern, i punkter. |
| [getWidthPixel()](#getWidthPixel--) | Returnerar eller anger bredden på den angivna slicern, i pixlar. |
| [getWorksheet()](#getWorksheet--) | Returnerar [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--)‑objektet som innehåller denna slicer. |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | Anger om slicer‑formen är låst. |
| [isPrintable()](#isPrintable--) | Anger om slicer‑objektet är utskrivbart. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Uppdaterar slicer‑objektets element från de associerade pivottabellerna. |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | Tar bort PivotTable‑anslutning. |
| [selectItems(String[] labels, boolean append)](#selectItems-java.lang.String---boolean-) | **Anmärkningar** |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Returnerar eller anger den beskrivande (alternativa) textsträngen för Slicer-objektet. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Returnerar eller anger rubriken för den angivna slicern. |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | Returnerar eller anger om rubriken som visar slicer‑rubriken är synlig. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Returnerar eller anger bredden på varje kolumn i slicern i enheten punkter. |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | Ställer in bredden på\\u807deach column i\\u807dthe slicer, i enhet av\\u807dpixels.\\u807d |
| [setFirstItemIndex(int value)](#setFirstItemIndex-int-) | Anger det nollbaserade indexet för det första slicer‑objektet. |
| [setHeight(double value)](#setHeight-double-) | Returnerar eller anger höjden på den angivna slicern, i punkter. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Returnerar eller anger höjden på den angivna slicern, i pixlar. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Returnerar eller anger den horisontella förskjutningen för slicer‑formen från dess vänstra kolumn, i pixlar. |
| [setLocked(boolean value)](#setLocked-boolean-) | Anger om slicer‑formen är låst. |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | Indikerar om bildförhållandet är låst. |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | Indikerar om den angivna slicern kan flyttas eller storleksändras via användargränssnittet. |
| [setName(String value)](#setName-java.lang.String-) | Returnerar eller anger namnet på den angivna slicern |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Returnerar eller anger antalet kolumner i slicern. |
| [setPlacement(int value)](#setPlacement-int-) | Representerar hur ritobjektet är fäst vid cellerna under det. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Anger om slicer‑objektet är utskrivbart. |
| [setRowHeight(double value)](#setRowHeight-double-) | Returnerar eller anger höjden på varje rad i den angivna slicern i enheten punkter. |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | Returnerar eller anger höjden på varje rad i den angivna slicern, i enheten pixlar. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Anger om alla objekt ska visas även om det inte finns någon data eller de har raderats. |
| [setShowCaption(boolean value)](#setShowCaption-boolean-) | Anger om slicer‑rubriken är synlig. |
| [setShowMissing(boolean value)](#setShowMissing-boolean-) | Anger om objekt som har tagits bort från datakällan ska visas. |
| [setShowTypeOfItemsWithNoData(int value)](#setShowTypeOfItemsWithNoData-int-) | Anger om objekt som har tagits bort från datakällan ska visas. |
| [setSortOrderType(int value)](#setSortOrderType-int-) | Anger typen av sorteringsobjekt. |
| [setStyleType(int value)](#setStyleType-int-) | Ange typen av inbyggd slicer‑stil. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Anger titeln på det aktuella Slicer‑objektet. |
| [setTopPixel(int value)](#setTopPixel-int-) | Returnerar eller anger det vertikala offsetet för slicer‑formen från dess översta rad, i pixlar. |
| [setWidth(double value)](#setWidth-double-) | Returnerar eller anger bredden på den angivna slicern, i punkter. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Returnerar eller anger bredden på den angivna slicern, i pixlar. |
| [toString()](#toString--) |  |
| [unselectItems(String[] labels)](#unselectItems-java.lang.String---) | Ta bort valda filteretiketter. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```


Lägger till PivotTable-anslutning.

**Example**

```
         slicer.addPivotConnection(pivot);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable‑objektet |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Ta bort filter

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Returnerar eller anger den beskrivande (alternativa) textsträngen för Slicer-objektet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) egenskap. Denna egenskap kommer att tas bort 12 månader senare, från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```


Returnerar eller anger rubriken för den angivna slicern.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```


Returnerar eller anger om rubriken som visar slicer‑Caption är synlig. Standardvärdet är true.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) egenskap. Denna egenskap kommer att tas bort 12 månader senare, från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Returnerar eller anger bredden på varje kolumn i slicern i enheten punkter.

**Example**

```
         slicer.setColumnWidth(80);
```

**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```


Hämtar bredden på\u807dvarje kolumn i\u807dslicern, i enheten\u807dpixlar.\u807d

**Example**

```
         slicer.setColumnWidthPixel(120);
```

**Returns:**
int
### getFirstItemIndex() {#getFirstItemIndex--}
```
public int getFirstItemIndex()
```


Anger det nollbaserade indexet för det första slicer‑objektet.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Returnerar eller anger höjden på den angivna slicern, i punkter.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Shape.HeightPt‑egenskap. Denna egenskap kommer att tas bort 12 månader senare, från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Returnerar eller anger höjden på den angivna slicern, i pixlar.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.Height. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Returnerar eller anger den horisontella förskjutningen för slicer‑formen från dess vänstra kolumn, i pixlar.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.Left. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```


Indikerar om bildförhållandet är låst.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) metod. Denna egenskap kommer att tas bort 12 månader senare, från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```


Indikerar om den angivna slicern kan flyttas eller storleksändras via användargränssnittet.

**Example**

```
         slicer.setLockedPosition(false);
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Returnerar eller anger namnet på den angivna slicern

**Example**

```
         slicer.setName("slicer name");
```

**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Returnerar eller anger antalet kolumner i slicern. Standardvärdet är 1.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```


Returnerar [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--)‑objektet som innehåller denna slicer. Skrivskyddad.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Representerar hur ritobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett kalkylblad.

Se [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Returnerar eller anger höjden på varje rad i den angivna slicern i enheten punkter.

**Example**

```
         slicer.setRowHeight(20);
```

**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```


Returnerar eller anger höjden på varje rad i den angivna slicern, i enheten pixlar.

**Example**

```
         slicer.setRowHeightPixel(30);
```

**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```


Returnerar Shape-objektet som är associerat med den angivna slicern. Endast läs.

**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Anger om alla objekt ska visas även om det inte finns någon data eller de har raderats. Standardvärdet är true;

**Returns:**
boolean
### getShowCaption() {#getShowCaption--}
```
public boolean getShowCaption()
```


Anger om slicerns rubrik är synlig. Standardvärdet är true

**Example**

```
         slicer.setShowCaption(false);
```

**Returns:**
boolean
### getShowMissing() {#getShowMissing--}
```
public boolean getShowMissing()
```


Anger om objekt som har tagits bort från datakällan ska visas.

**Remarks**

Fungerar endast när [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) är true.

**Returns:**
boolean
### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}
```
public int getShowTypeOfItemsWithNoData()
```


Anger om objekt som har tagits bort från datakällan ska visas.

Se [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Fungerar endast när [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) är true.

**Returns:**
int
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```


Returnerar SlicerCache-objektet som är associerat med slicern. Endast läs.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getSortOrderType() {#getSortOrderType--}
```
public int getSortOrderType()
```


Anger typen av sorteringsobjekt.

Se [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```


Ange typen av inbyggd slicer-stil. Standardtypen är SlicerStyleLight1.

Se [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Example**

```
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```

**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```


Anger titeln på det aktuella Slicer‑objektet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Returnerar eller anger det vertikala offsetet för slicer‑formen från dess översta rad, i pixlar.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället Shape.Top-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Returnerar eller anger bredden på den angivna slicern, i punkter.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Shape.WidthPt egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Returnerar eller anger bredden på den angivna slicern, i pixlar.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället Shape.Width-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Returnerar [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--)‑objektet som innehåller denna slicer. Skrivskyddad.

**Example**

```
         Worksheet currSheet = slicer.getParent();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Anger om slicer‑formen är låst.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Anger om slicer‑objektet är utskrivbart.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         slicer.removePivotConnection(pivot);
```

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




### refresh() {#refresh--}
```
public void refresh()
```


Uppdaterar slicer‑objektets element från de associerade pivottabellerna.

**Example**

```
         slicer.refresh();
```

### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```


Tar bort PivotTable‑anslutning.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable‑objektet |

### selectItems(String[] labels, boolean append) {#selectItems-java.lang.String---boolean-}
```
public void selectItems(String[] labels, boolean append)
```


**Remarks**

Om du vill markera alla objekt, använd [clearFilter()](../../com.aspose.cells/slicer\#clearFilter--) metod.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| etiketter | java.lang.String[] | Valda etiketter. |
| lägg till | boolean | False betyder att endast dessa etiketter markeras och övriga avmarkeras. True betyder att befintliga markerade objekt behålls och dessa etiketter markeras. |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Returnerar eller anger den beskrivande (alternativa) textsträngen för Slicer-objektet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) egenskap. Denna egenskap kommer att tas bort 12 månader senare, från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Returnerar eller anger rubriken för den angivna slicern.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```


Returnerar eller anger om rubriken som visar slicer‑Caption är synlig. Standardvärdet är true.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) egenskap. Denna egenskap kommer att tas bort 12 månader senare, från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Returnerar eller anger bredden på varje kolumn i slicern i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```


Ställer in bredden på\\u807deach column i\\u807dthe slicer, i enhet av\\u807dpixels.\\u807d

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFirstItemIndex(int value) {#setFirstItemIndex-int-}
```
public void setFirstItemIndex(int value)
```


Anger det nollbaserade indexet för det första slicer‑objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Returnerar eller anger höjden på den angivna slicern, i punkter.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Shape.HeightPt‑egenskap. Denna egenskap kommer att tas bort 12 månader senare, från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Returnerar eller anger höjden på den angivna slicern, i pixlar.

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


Returnerar eller anger den horisontella förskjutningen för slicer‑formen från dess vänstra kolumn, i pixlar.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.Left. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Anger om slicer‑formen är låst.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```


Indikerar om bildförhållandet är låst.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) metod. Denna egenskap kommer att tas bort 12 månader senare, från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```


Indikerar om den angivna slicern kan flyttas eller storleksändras via användargränssnittet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Returnerar eller anger namnet på den angivna slicern

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Returnerar eller anger antalet kolumner i slicern. Standardvärdet är 1.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Representerar hur ritobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett kalkylblad.

Se [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Anger om slicer‑objektet är utskrivbart.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Returnerar eller anger höjden på varje rad i den angivna slicern i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```


Returnerar eller anger höjden på varje rad i den angivna slicern, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Anger om alla objekt ska visas även om det inte finns någon data eller de har raderats. Standardvärdet är true;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowCaption(boolean value) {#setShowCaption-boolean-}
```
public void setShowCaption(boolean value)
```


Anger om slicerns rubrik är synlig. Standardvärdet är true

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowMissing(boolean value) {#setShowMissing-boolean-}
```
public void setShowMissing(boolean value)
```


Anger om objekt som har tagits bort från datakällan ska visas.

**Remarks**

Fungerar endast när [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowTypeOfItemsWithNoData(int value) {#setShowTypeOfItemsWithNoData-int-}
```
public void setShowTypeOfItemsWithNoData(int value)
```


Anger om objekt som har tagits bort från datakällan ska visas.

Se [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Fungerar endast när [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSortOrderType(int value) {#setSortOrderType-int-}
```
public void setSortOrderType(int value)
```


Anger typen av sorteringsobjekt.

Se [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```


Ange typen av inbyggd slicer-stil. Standardtypen är SlicerStyleLight1.

Se [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Anger titeln på det aktuella Slicer‑objektet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Returnerar eller anger det vertikala offsetet för slicer‑formen från dess översta rad, i pixlar.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället Shape.Top-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Returnerar eller anger bredden på den angivna slicern, i punkter.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Shape.WidthPt egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Returnerar eller anger bredden på den angivna slicern, i pixlar.

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
### unselectItems(String[] labels) {#unselectItems-java.lang.String---}
```
public void unselectItems(String[] labels)
```


Ta bort valda filteretiketter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| etiketter | java.lang.String[] | Etiketterna. |

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

