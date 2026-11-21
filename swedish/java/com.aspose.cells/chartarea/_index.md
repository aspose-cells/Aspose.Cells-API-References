---
title: "ChartArea"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar diagramområdet i kalkylbladet."
type: docs
url: /sv/java/com.aspose.cells/chartarea/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe)
```
public class ChartArea extends ChartFrame
```

Inkapslar objektet som representerar diagramområdet i kalkylbladet.

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
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Getting Chart Area
         ChartArea chartArea = chart.getChartArea();
 
         //Setting the foreground color of the chart area
         chartArea.getArea().setForegroundColor(Color.getYellow());
 
         //Setting Chart Area Shadow
         chartArea.setShadow(true);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Hämtar [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. |
| [getBackground()](#getBackground--) | Hämtar bakgrundens visningsläge. |
| [getBackgroundMode()](#getBackgroundMode--) | Hämtar bakgrundens visningsläge. |
| [getBorder()](#getBorder--) | Hämtar [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Hämtar diagrammet som detta objekt tillhör. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Representerar höjden för standardpositionen i enheter av 1/4000 av diagramområdet. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | Representerar höjden för standardpositionen i enheter av bråkdelen av diagramområdet. |
| [getDefaultWidth()](#getDefaultWidth--) | Representerar bredden för standardpositionen i enheter av 1/4000 av diagramområdet. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | Representerar bredden för standardpositionen i enheter av bråkdelen av diagramområdet. |
| [getDefaultX()](#getDefaultX--) | Representerar x för standardpositionen i enheter av 1/4000 av diagramområdet. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | Representerar x för standardpositionen i enheter av bråkdelen av diagramområdet. |
| [getDefaultY()](#getDefaultY--) | Representerar y för standardpositionen i enheter av 1/4000 av diagramområdet. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | Representerar y för standardpositionen i enheter av bråkdelen av diagramområdet. |
| [getFont()](#getFont--) | Hämtar ett [getFont()](../../com.aspose.cells/chartarea\#getFont--)‑objekt för det angivna ChartArea‑objektet. |
| [getHeight()](#getHeight--) | Hämtar den vertikala förskjutningen från dess nedre\u9225\u6186ight hörnrad, i enheter av 1/4000 av diagramområdet. |
| [getHeightPixel()](#getHeightPixel--) | Hämtar ramens höjd i enheter av pixlar. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Hämtar den vertikala förskjutningen från dess nedre högra hörnrad, i enheter av förhållandet till diagramområdet. |
| [getShadow()](#getShadow--) | Sant om ramen har en skugga. |
| [getShapeProperties()](#getShapeProperties--) | Hämtar [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) objektet. |
| [getTextFont()](#getTextFont--) | Hämtar ett [getFont()](../../com.aspose.cells/chartframe\#getFont--) objekt av det angivna ChartFrame-objektet. |
| [getTextOptions()](#getTextOptions--) | Hämtar textens alternativ. |
| [getWidth()](#getWidth--) | Hämtar den horisontella förskjutningen från dess nedre högra hörnkolumn, i enheter av 1/4000 av diagramområdet. |
| [getWidthPixel()](#getWidthPixel--) | Hämtar ramens bredd i enheter av pixel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Hämtar den horisontella förskjutningen från dess nedre högra hörnkolumn, i enheter av förhållandet till diagramområdet. |
| [getX()](#getX--) | Hämtar den horisontella förskjutningen från dess övre‑vänstra hörnkolumn, i enheter av 1/4000 av diagramområdet. |
| [getXPixel()](#getXPixel--) | Hämtar x‑koordinaten för det övre vänstra hörnet i enheter av pixel. |
| [getXRatioToChart()](#getXRatioToChart--) | Hämtar den horisontella förskjutningen från den övre‑vänstra hörnkolumnen, som ett förhållande till diagramområdet. |
| [getY()](#getY--) | Hämtar eller sätter den vertikala förskjutningen från dess övre vänstra hörnrad, i enheter av 1/4000 av diagramområdet. |
| [getYPixel()](#getYPixel--) | Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [getYRatioToChart()](#getYRatioToChart--) | Hämtar eller sätter den vertikala förskjutningen från dess övre vänstra hörnrad, i enheter av förhållandet till diagramområdet. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticSize()](#isAutomaticSize--) | Indikerar om diagramramen har automatisk storlek. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indikerar om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är angiven. |
| [isInnerMode()](#isInnerMode--) | Indikerar om storleken på plotområdet inkluderar tick-markeringar och axelrubriker. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indikerar om diagramramen har automatisk storlek. |
| [setBackground(int value)](#setBackground-int-) | Ställer in bakgrundens visningsläge. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Ställer in bakgrundens visningsläge. |
| [setHeight(int value)](#setHeight-int-) | Ställer in den vertikala förskjutningen från dess nedre\u9225\u6186ight hörnrad, i enheter av 1/4000 av diagramområdet. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Ställer in ramens höjd i enheter av pixlar. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Ställer in den vertikala förskjutningen från dess nedre högra hörnrad, i enheter av förhållandet till diagramområdet. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indikerar om storleken på plotområdet inkluderar tick-markeringar och axelrubriker. |
| [setPositionAuto()](#setPositionAuto--) | Ställ in ramens position till automatisk |
| [setShadow(boolean value)](#setShadow-boolean-) | Sant om ramen har en skugga. |
| [setWidth(int value)](#setWidth-int-) | Ställer in den horisontella förskjutningen från dess nedre högra hörnkolumn, i enheter av 1/4000 av diagramområdet. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Ställer in bredden på ramen i enheter av pixel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Ställer in den horisontella förskjutningen från dess nedre högra hörnkolumn, i enheter av förhållandet till diagramområdet. |
| [setX(int value)](#setX-int-) | Ställer in den horisontella förskjutningen från dess övre‑vänstra hörnkolumn, i enheter av 1/4000 av diagramområdet. |
| [setXPixel(int value)](#setXPixel-int-) | Ställer in x-koordinaten för det övre vänstra hörnet i enheter av pixel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Ställer in den horisontella förskjutningen från den övre‑vänstra hörnkolumnen, som ett förhållande till diagramområdet. |
| [setY(int value)](#setY-int-) | Hämtar eller sätter den vertikala förskjutningen från dess övre vänstra hörnrad, i enheter av 1/4000 av diagramområdet. |
| [setYPixel(int value)](#setYPixel-int-) | Ställer in y-koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Hämtar eller sätter den vertikala förskjutningen från dess övre vänstra hörnrad, i enheter av förhållandet till diagramområdet. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Hämtar [getArea()](../../com.aspose.cells/chartframe\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


Hämtar bakgrundens visningsläge. Denna egenskap är endast giltig i Excel 2003 eller tidigare versioner.

Se [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.Area.FillFormat.FillType. Till exempel, om du behöver ställa in BackgroundMode till Opaque, kan du använda följande kod: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Denna egenskap kommer att tas bort 12 månader senare sedan JANUARY 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Hämtar bakgrundens visningsläge. Denna egenskap är endast giltig i Excel 2003 eller tidigare versioner.

Se [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.Area.FillFormat.FillType. Till exempel, om du behöver ställa in BackgroundMode till Opaque, kan du använda följande kod: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Denna egenskap kommer att tas bort 12 månader senare sedan februari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Hämtar [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


Hämtar diagrammet som detta objekt tillhör.

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultHeight() {#getDefaultHeight--}
```
public int getDefaultHeight()
```


Representerar höjden för standardpositionen i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.DefaultHeightRatioToChart. DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); Denna egenskap kommer att tas bort 12 månader senare sedan februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


Representerar höjden för standardpositionen i enheter av bråkdelen av diagramområdet.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Representerar bredden för standardpositionen i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.DefaultWidthRatioToChart. DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); Denna egenskap kommer att tas bort 12 månader senare sedan februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


Representerar bredden för standardpositionen i enheter av bråkdelen av diagramområdet.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Representerar x för standardpositionen i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.DefaultXRatioToChart. DefaultX = (int)(DefaultXRatioToChart \* 4000); Denna egenskap kommer att tas bort 12 månader senare sedan februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


Representerar x för standardpositionen i enheter av bråkdelen av diagramområdet.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Representerar y för standardpositionen i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.DefaultYRatioToChart. DefaultY = (int)(DefaultYRatioToChart \* 4000); Denna egenskap kommer att tas bort 12 månader senare sedan februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


Representerar y för standardpositionen i enheter av bråkdelen av diagramområdet.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Hämtar ett [getFont()](../../com.aspose.cells/chartarea\#getFont--)‑objekt för det angivna ChartArea‑objektet.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Hämtar den vertikala förskjutningen från dess nedre\u9225\u6186ight hörnrad, i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartArea.HeightRatioToChart. Height = HeightRatioToChart \* 4000. Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Hämtar ramens höjd i enheter av pixlar.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


Hämtar den vertikala förskjutningen från dess nedre högra hörnrad, i enheter av förhållandet till diagramområdet.

**Returns:**
double
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Sant om ramen har en skugga.

**Remarks**

Endast för diagram i xls‑fil.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Hämtar [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) objektet.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Hämtar ett [getFont()](../../com.aspose.cells/chartframe\#getFont--) objekt av det angivna ChartFrame-objektet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället ChartFrame.Font‑egenskapen. Den här egenskapen kommer att tas bort 12 månader senare från och med januari 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Hämtar textens alternativ.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getWidth() {#getWidth--}
```
public int getWidth()
```


Hämtar den horisontella förskjutningen från dess nedre högra hörnkolumn, i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartArea.WidthRatioToChart. Width = WidthRatioToChart \* 4000. Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Hämtar ramens bredd i enheter av pixel.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


Hämtar den horisontella förskjutningen från dess nedre högra hörnkolumn, i enheter av förhållandet till diagramområdet.

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Hämtar den horisontella förskjutningen från dess övre‑vänstra hörnkolumn, i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartArea.XRatioToChart. X = XRatioToChart \* 4000. Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Hämtar x‑koordinaten för det övre vänstra hörnet i enheter av pixel.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


Hämtar den horisontella förskjutningen från den övre‑vänstra hörnkolumnen, som ett förhållande till diagramområdet.

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Hämtar eller sätter den vertikala förskjutningen från dess övre vänstra hörnrad, i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartArea.YRatioToChart. Y = YRatioToChart \* 4000; Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av pixlar.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


Hämtar eller sätter den vertikala förskjutningen från dess övre vänstra hörnrad, i enheter av förhållandet till diagramområdet.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Indikerar om diagramramen har automatisk storlek.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Indikerar om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är angiven.

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Anger om storleken på plotområdet inkluderar tick‑markeringarna och axel‑etiketterna. False betyder att storleken ska bestämma storleken på plotområdet, tick‑markeringarna och axel‑etiketterna.

**Remarks**

Endast för Xlsx‑fil.

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Indikerar om diagramramen har automatisk storlek.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


Ställer in bakgrundens visningsläge. Den här egenskapen är endast giltig i Excel 2003 eller tidigare versioner.

Se [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.Area.FillFormat.FillType. Till exempel, om du behöver ställa in BackgroundMode till Opaque, kan du använda följande kod: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Denna egenskap kommer att tas bort 12 månader senare sedan JANUARY 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Ställer in bakgrundens visningsläge. Den här egenskapen är endast giltig i Excel 2003 eller tidigare versioner.

Se [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.Area.FillFormat.FillType. Till exempel, om du behöver ställa in BackgroundMode till Opaque, kan du använda följande kod: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Denna egenskap kommer att tas bort 12 månader senare sedan februari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Ställer in den vertikala förskjutningen från dess nedre\u9225\u6186ight hörnrad, i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartArea.HeightRatioToChart. Height = HeightRatioToChart \* 4000. Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Ställer in ramens höjd i enheter av pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


Ställer in den vertikala förskjutningen från dess nedre högra hörnrad, i enheter av förhållandet till diagramområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Anger om storleken på plotområdet inkluderar tick‑markeringarna och axel‑etiketterna. False betyder att storleken ska bestämma storleken på plotområdet, tick‑markeringarna och axel‑etiketterna.

**Remarks**

Endast för Xlsx‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Ställ in ramens position till automatisk

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Sant om ramen har en skugga.

**Remarks**

Endast för diagram i xls‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Ställer in den horisontella förskjutningen från dess nedre högra hörnkolumn, i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartArea.WidthRatioToChart. Width = WidthRatioToChart \* 4000. Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Ställer in bredden på ramen i enheter av pixel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


Ställer in den horisontella förskjutningen från dess nedre högra hörnkolumn, i enheter av förhållandet till diagramområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Ställer in den horisontella förskjutningen från dess övre‑vänstra hörnkolumn, i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartArea.XRatioToChart. X = XRatioToChart \* 4000. Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Ställer in x-koordinaten för det övre vänstra hörnet i enheter av pixel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


Ställer in den horisontella förskjutningen från den övre‑vänstra hörnkolumnen, som ett förhållande till diagramområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Hämtar eller sätter den vertikala förskjutningen från dess övre vänstra hörnrad, i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartArea.YRatioToChart. Y = YRatioToChart \* 4000; Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Ställer in y-koordinaten för det övre vänstra hörnet i enheter av pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


Hämtar eller sätter den vertikala förskjutningen från dess övre vänstra hörnrad, i enheter av förhållandet till diagramområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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

