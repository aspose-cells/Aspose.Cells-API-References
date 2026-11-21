---
title: "SparklineGroup"
second_title: "Aspose.Cells för Java API-referens"
description: "är organiserad i en sparkline-grupp."
type: docs
url: /sv/java/com.aspose.cells/sparklinegroup/
---

**Inheritance:**
java.lang.Object
```
public class SparklineGroup
```

[Sparkline](../../com.aspose.cells/sparkline) is organized into a sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         // Create CellsColor
         CellsColor clr = book.createCellsColor();
         clr.setColor(Color.getOrange());
         group.setSeriesColor(clr);
 
         // set the high points are colored green and the low points are colored red
         group.setShowHighPoint(true);
         group.setShowLowPoint(true);
         group.getHighPointColor().setColor(Color.getGreen());
         group.getLowPointColor().setColor(Color.getRed());
         // set line weight 
         group.setLineWeight(1.0);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | Anger om data ska visas i dolda rader och kolumner. |
| [getFirstPointColor()](#getFirstPointColor--) | Hämtar färgen på den första datapunkten i sparkline-gruppen. |
| [getHighPointColor()](#getHighPointColor--) | Hämtar färgen på de högsta datapunkterna i sparkline-gruppen. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | Hämtar färgen på den horisontella axeln i sparkline-gruppen. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | Representerar intervallet som innehåller datumvärdena för sparkline-data. |
| [getLastPointColor()](#getLastPointColor--) | Hämtar färgen på den sista datapunkten i sparkline-gruppen. |
| [getLineWeight()](#getLineWeight--) | Hämtar linjebredden i varje linjesparkline i sparkline-gruppen, i enheten punkter. |
| [getLowPointColor()](#getLowPointColor--) | Hämtar färgen på de lägsta datapunkterna i sparkline-gruppen. |
| [getMarkersColor()](#getMarkersColor--) | Hämtar färgen på punkterna i varje linjesparkline i sparkline-gruppen. |
| [getNegativePointsColor()](#getNegativePointsColor--) | Hämtar färgen på de negativa värdena i sparkline-gruppen. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Anger hur tomma celler ska plottas. |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | Anger om plottdatan är från höger till vänster. |
| [getPresetStyle()](#getPresetStyle--) | Hämtar den förinställda stiltypen för sparkline-gruppen. |
| [getSeriesColor()](#getSeriesColor--) | Hämtar färgen på sparkline-diagrammen i sparkline-gruppen. |
| [getShowFirstPoint()](#getShowFirstPoint--) | Anger om den första datapunkten i sparkline-gruppen ska markeras. |
| [getShowHighPoint()](#getShowHighPoint--) | Anger om de högsta datapunkterna i sparkline-gruppen ska markeras. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | Anger om den horisontella axeln för sparkline ska visas. |
| [getShowLastPoint()](#getShowLastPoint--) | Anger om den sista datapunkten i sparkline-gruppen ska markeras. |
| [getShowLowPoint()](#getShowLowPoint--) | Anger om de lägsta datapunkterna i sparkline-gruppen ska markeras. |
| [getShowMarkers()](#getShowMarkers--) | Anger om varje punkt i varje linjesparkline i sparkline-gruppen ska markeras. |
| [getShowNegativePoints()](#getShowNegativePoints--) | Anger om de negativa värdena i sparkline-gruppen ska markeras med en annan färg eller markör. |
| [getSparklineCollection()](#getSparklineCollection--) | Hämtar samlingen av [Sparkline](../../com.aspose.cells/sparkline)-objekt. |
| [getSparklines()](#getSparklines--) | Hämtar samlingen av [Sparkline](../../com.aspose.cells/sparkline)-objekt. |
| [getType()](#getType--) | Anger sparklinetypen för sparkline-gruppen. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | Hämtar det anpassade maximala värdet för den vertikala axeln. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | Representerar typen av maximalt värde för den vertikala axeln. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | Hämtar det anpassade minimala värdet för den vertikala axeln. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | Representerar typen av minimalt värde för den vertikala axeln. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | Återställer dataområdet och positionsområdet för sparkline-gruppen. |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | Anger om data ska visas i dolda rader och kolumner. |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | Ställer in färgen på den första datapunkten i sparkline-gruppen. |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | Ställer in färgen på de högsta datapunkterna i sparkline-gruppen. |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | Ställer in färgen på den horisontella axeln i sparkline-gruppen. |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | Representerar intervallet som innehåller datumvärdena för sparkline-data. |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | Ställer in färgen på den sista datapunkten i sparkline-gruppen. |
| [setLineWeight(double value)](#setLineWeight-double-) | Ställer in linjebredden i varje linjesparkline i sparkline-gruppen, i enheten punkter. |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | Ställer in färgen på de lägsta datapunkterna i sparkline-gruppen. |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | Ställer in färgen på punkterna i varje linjesparkline i sparkline-gruppen. |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | Ställer in färgen på de negativa värdena i sparkline-gruppen. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Anger hur tomma celler ska plottas. |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | Anger om plottdatan är från höger till vänster. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Ställer in den förinställda stiltypen för sparkline-gruppen. |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | Ställer in färgen på sparkline-diagrammen i sparkline-gruppen. |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | Anger om den första datapunkten i sparkline-gruppen ska markeras. |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | Anger om de högsta datapunkterna i sparkline-gruppen ska markeras. |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | Anger om den horisontella axeln för sparkline ska visas. |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | Anger om den sista datapunkten i sparkline-gruppen ska markeras. |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | Anger om de lägsta datapunkterna i sparkline-gruppen ska markeras. |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | Anger om varje punkt i varje linjesparkline i sparkline-gruppen ska markeras. |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | Anger om de negativa värdena i sparkline-gruppen ska markeras med en annan färg eller markör. |
| [setType(int value)](#setType-int-) | Anger sparklinetypen för sparkline-gruppen. |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | Ställer in det anpassade maximala värdet för den vertikala axeln. |
| [setVerticalAxisMaxValue(int type, double value)](#setVerticalAxisMaxValue-int-double-) | Ställer in det anpassade maximala värdet för sparkline-axeln med den angivna axelvärdestypen. |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | Representerar typen av maximalt värde för den vertikala axeln. |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | Ställer in det anpassade minimivärdet för den vertikala axeln. |
| [setVerticalAxisMinValue(int type, double value)](#setVerticalAxisMinValue-int-double-) | Ställer in det anpassade minimivärdet för sparkline‑axelns vertikala axel med den angivna axelvärdestypen. |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | Representerar typen av minimalt värde för den vertikala axeln. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDisplayHidden() {#getDisplayHidden--}
```
public boolean getDisplayHidden()
```


Anger om data ska visas i dolda rader och kolumner.

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


Hämtar färgen på den första datapunkten i sparkline-gruppen.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


Hämtar färgen på de högsta datapunkterna i sparkline-gruppen.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


Hämtar färgen på den horisontella axeln i sparkline-gruppen.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


Representerar intervallet som innehåller datumvärdena för sparkline-data.

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


Hämtar färgen på den sista datapunkten i sparkline-gruppen.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


Hämtar linjebredden i varje linjesparkline i sparkline-gruppen, i enheten punkter.

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


Hämtar färgen på de lägsta datapunkterna i sparkline-gruppen.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


Hämtar färgen på punkterna i varje linjesparkline i sparkline-gruppen.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


Hämtar färgen på de negativa värdena i sparkline-gruppen.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Anger hur tomma celler ska plottas.

Se [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


Anger om plottdatan är från höger till vänster.

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Hämtar den förinställda stiltypen för sparkline-gruppen.

Se [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Om den här egenskapen är inställd, kommer dessa egenskaper: SeriesColor, NegativePointsColor, HorizontalAxisColor, MarkersColor, FirstPointColor, LastPointColor, HighPointColor, LowPointColor att täckas. Så vänligen sätt egenskapen först, sedan sätt de andra.

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


Hämtar färgen på sparkline-diagrammen i sparkline-gruppen.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


Anger om den första datapunkten i sparkline-gruppen ska markeras.

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


Anger om de högsta datapunkterna i sparkline-gruppen ska markeras.

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


Anger om den horisontella axeln för sparkline ska visas. Den horisontella axeln visas om sparkline har data som korsar nollaxeln.

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


Anger om den sista datapunkten i sparkline-gruppen ska markeras.

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


Anger om de lägsta datapunkterna i sparkline-gruppen ska markeras.

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


Anger om varje punkt i varje linjesparkline i sparkline-gruppen ska markeras.

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


Anger om de negativa värdena i sparkline-gruppen ska markeras med en annan färg eller markör.

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


Hämtar samlingen av [Sparkline](../../com.aspose.cells/sparkline)-objekt.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd i stället egenskapen SparklineGroup.Sparklines. Denna egenskap kommer att tas bort 12 månader senare från och med november 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


Hämtar samlingen av [Sparkline](../../com.aspose.cells/sparkline)-objekt.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


Anger sparklinetypen för sparkline-gruppen.

Se [SparklineType](../../com.aspose.cells/sparklinetype).

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


Hämtar det anpassade maximala värdet för den vertikala axeln.

**Remarks**

Om den här egenskapen är inställd, kommer [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) att vara [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


Representerar typen av maximalt värde för den vertikala axeln.

Se [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


Hämtar det anpassade minimala värdet för den vertikala axeln.

**Remarks**

Om den här egenskapen är inställd, kommer [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) att vara [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


Representerar typen av minimalt värde för den vertikala axeln.

Se [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

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




### resetRanges(String dataRange, boolean isVertical, CellArea locationRange) {#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public void resetRanges(String dataRange, boolean isVertical, CellArea locationRange)
```


Återställer dataområdet och placeringsområdet för sparkline‑gruppen. Denna metod rensar ursprungliga sparkline‑objekt i gruppen och skapar nya sparkline‑objekt för de nya områdena.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataRange | java.lang.String | Anger det nya dataområdet för sparkline‑gruppen. |
| isVertical | boolean | Anger om sparklines ska plottas från det nya dataområdet radvis eller kolumnvis. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Anger var sparklines ska placeras. |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


Anger om data ska visas i dolda rader och kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


Ställer in färgen på den första datapunkten i sparkline-gruppen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


Ställer in färgen på de högsta datapunkterna i sparkline-gruppen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


Ställer in färgen på den horisontella axeln i sparkline-gruppen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


Representerar intervallet som innehåller datumvärdena för sparkline-data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


Ställer in färgen på den sista datapunkten i sparkline-gruppen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


Ställer in linjebredden i varje linjesparkline i sparkline-gruppen, i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


Ställer in färgen på de lägsta datapunkterna i sparkline-gruppen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


Ställer in färgen på punkterna i varje linjesparkline i sparkline-gruppen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


Ställer in färgen på de negativa värdena i sparkline-gruppen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Anger hur tomma celler ska plottas.

Se [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


Anger om plottdatan är från höger till vänster.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Ställer in den förinställda stiltypen för sparkline-gruppen.

Se [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Om den här egenskapen är inställd, kommer dessa egenskaper: SeriesColor, NegativePointsColor, HorizontalAxisColor, MarkersColor, FirstPointColor, LastPointColor, HighPointColor, LowPointColor att täckas. Så vänligen sätt egenskapen först, sedan sätt de andra.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


Ställer in färgen på sparkline-diagrammen i sparkline-gruppen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


Anger om den första datapunkten i sparkline-gruppen ska markeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


Anger om de högsta datapunkterna i sparkline-gruppen ska markeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


Anger om den horisontella axeln för sparkline ska visas. Den horisontella axeln visas om sparkline har data som korsar nollaxeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


Anger om den sista datapunkten i sparkline-gruppen ska markeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


Anger om de lägsta datapunkterna i sparkline-gruppen ska markeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


Anger om varje punkt i varje linjesparkline i sparkline-gruppen ska markeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


Anger om de negativa värdena i sparkline-gruppen ska markeras med en annan färg eller markör.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Anger sparklinetypen för sparkline-gruppen.

Se [SparklineType](../../com.aspose.cells/sparklinetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


Ställer in det anpassade maximala värdet för den vertikala axeln.

**Remarks**

Om den här egenskapen är inställd, kommer [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) att vara [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setVerticalAxisMaxValue(int type, double value) {#setVerticalAxisMaxValue-int-double-}
```
public void setVerticalAxisMaxValue(int type, double value)
```


Ställer in det anpassade maximala värdet för sparkline-axeln med den angivna axelvärdestypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Typ som anger hur axelns maximala värde tillämpas. |
| value | double | Anpassat maximalt värde för den vertikala axeln. Ignoreras om typen inte är [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


Representerar typen av maximalt värde för den vertikala axeln.

Se [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


Ställer in det anpassade minimivärdet för den vertikala axeln.

**Remarks**

Om den här egenskapen är inställd, kommer [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) att vara [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setVerticalAxisMinValue(int type, double value) {#setVerticalAxisMinValue-int-double-}
```
public void setVerticalAxisMinValue(int type, double value)
```


Ställer in det anpassade minimivärdet för sparkline‑axelns vertikala axel med den angivna axelvärdestypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Typ som anger hur axelns minimala värde tillämpas. |
| value | double | Anpassat minimalt värde för den vertikala axeln. Ignoreras om typen inte är [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


Representerar typen av minimalt värde för den vertikala axeln.

Se [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

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

