---
title: "ChartDataTable"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en diagramdatatabell."
type: docs
url: /sv/java/com.aspose.cells/chartdatatable/
---

**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```

Representerar en diagramdatatabell.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
 
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
 
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
 
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
 
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
 
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
 
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         chart.setShowDataTable(true);
 
         //Getting Chart Table
         ChartDataTable chartTable = chart.getChartDataTable();
 
         //Setting Chart Table Font Color
         chartTable.getFont().setColor(com.aspose.cells.Color.getRed());
 
         //Setting Legend Key VisibilityOptions
         chartTable.setShowLegendKey(false);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. |
| [getBackgroundMode()](#getBackgroundMode--) | Hämtar visningsläget för bakgrunden |
| [getBorder()](#getBorder--) | Returnerar ett Border-objekt som representerar objektets kant. |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Hämtar ett [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) objekt som representerar teckensnittsinställningen för den angivna diagramdatatabellen. |
| [getShowLegendKey()](#getShowLegendKey--) | Sant om nyckeln för datalabellegenden är synlig. |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | Sant om diagramdatatabellen har horisontella cellkantlinjer |
| [hasBorderOutline()](#hasBorderOutline--) | Sant om diagramdatatabellen har konturkanter |
| [hasBorderVertical()](#hasBorderVertical--) | Sant om diagrammets datatabell har vertikala cellramar |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | Sant om diagramdatatabellen har horisontella cellkantlinjer |
| [hasOutlineBorder()](#hasOutlineBorder--) | Sant om diagramdatatabellen har konturkanter |
| [hasVerticalBorder()](#hasVerticalBorder--) | Sant om diagrammets datatabell har vertikala cellramar |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Ställer in visningsläget för bakgrunden |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | Sant om diagramdatatabellen har horisontella cellkantlinjer |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | Sant om diagramdatatabellen har konturkanter |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | Sant om diagrammets datatabell har vertikala cellramar |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | Sant om diagramdatatabellen har horisontella cellkantlinjer |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | Sant om diagramdatatabellen har konturkanter |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | Sant om diagrammets datatabell har vertikala cellramar |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Sant om nyckeln för datalabellegenden är synlig. |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant.

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Hämtar visningsläget för bakgrunden

Se [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Returnerar ett Border-objekt som representerar objektets kant.

**Returns:**
[Line](../../com.aspose.cells/line)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


Hämtar ett [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) objekt som representerar teckensnittsinställningen för den angivna diagramdatatabellen.

**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Sant om nyckeln för datalabellegenden är synlig.

**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```


Sant om diagramdatatabellen har horisontella cellkantlinjer

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ChartDataTable.HasHorizontalBorder. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```


Sant om diagramdatatabellen har konturkanter

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ChartDataTable.HasOutlineBorder. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```


Sant om diagrammets datatabell har vertikala cellramar

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ChartDataTable.HasVerticalBorder. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```


Sant om diagramdatatabellen har horisontella cellkantlinjer

**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```


Sant om diagramdatatabellen har konturkanter

**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```


Sant om diagrammets datatabell har vertikala cellramar

**Returns:**
boolean
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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Ställer in visningsläget för bakgrunden

Se [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```


Sant om diagramdatatabellen har horisontella cellkantlinjer

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ChartDataTable.HasHorizontalBorder. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```


Sant om diagramdatatabellen har konturkanter

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ChartDataTable.HasOutlineBorder. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```


Sant om diagrammets datatabell har vertikala cellramar

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ChartDataTable.HasVerticalBorder. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```


Sant om diagramdatatabellen har horisontella cellkantlinjer

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```


Sant om diagramdatatabellen har konturkanter

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```


Sant om diagrammets datatabell har vertikala cellramar

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Sant om nyckeln för datalabellegenden är synlig.

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

