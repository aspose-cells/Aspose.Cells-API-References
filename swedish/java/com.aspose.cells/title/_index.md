---
title: "Titel"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar titeln på diagrammet eller axeln."
type: docs
url: /sv/java/com.aspose.cells/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class Title extends ChartTextFrame
```

Inkapslar objektet som representerar titeln på diagrammet eller axeln.

**Example**

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
         	Chart chart = sheet.getCharts().get(chartIndex);
 
         //Setting the title of a chart
         chart.getTitle().setText("Title");
         //Setting the font color of the chart title to blue
         chart.getTitle().getFont().setColor(Color.getBlue());
         //Setting the title of category axis of the chart
         chart.getCategoryAxis().getTitle().setText("Category");
         //Setting the title of value axis of the chart
         chart.getValueAxis().getTitle().setText("Value");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [characters()](#characters--) | Hämtar rik textformatering för denna Titel. |
| [characters(int startIndex, int length)](#characters-int-int-) | Returnerar ett Characters-objekt som representerar ett intervall av tecken inom texten. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Hämtar [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. |
| [getBackground()](#getBackground--) | Hämtar bakgrundens visningsläge. |
| [getBackgroundMode()](#getBackgroundMode--) | Hämtar bakgrundens visningsläge. |
| [getBorder()](#getBorder--) | Hämtar [Line](../../com.aspose.cells/line). |
| [getCharacters()](#getCharacters--) | Hämtar rik textformatering för denna Titel. |
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
| [getDirectionType()](#getDirectionType--) | Hämtar textens riktning. |
| [getFont()](#getFont--) | Hämtar ett [getFont()](../../com.aspose.cells/chartframe\#getFont--) objekt av det angivna ChartFrame-objektet. |
| [getHeight()](#getHeight--) | Hämtar ramens höjd i enheter av 1/4000 av diagramområdet. |
| [getHeightPixel()](#getHeightPixel--) | Hämtar ramens höjd i enheter av pixlar. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Hämtar ramens höjd i enheter av förhållandet till diagramområdet. |
| [getLinkedSource()](#getLinkedSource--) | Hämtar en referens till arbetsbladet. |
| [getOverLay()](#getOverLay--) | Representerar en överlagrad centrerad titel på ett diagram utan att ändra diagrammets storlek. |
| [getReadingOrder()](#getReadingOrder--) | Representerar textens läsriktning. |
| [getRotationAngle()](#getRotationAngle--) | Representerar textens rotationsvinkel. |
| [getShadow()](#getShadow--) | Sant om ramen har en skugga. |
| [getShapeProperties()](#getShapeProperties--) | Hämtar [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) objektet. |
| [getText()](#getText--) | Hämtar texten för visningsenhetsetiketten. |
| [getTextDirection()](#getTextDirection--) | Representerar textens läsriktning. |
| [getTextFont()](#getTextFont--) | Hämtar ett [getFont()](../../com.aspose.cells/chartframe\#getFont--) objekt av det angivna ChartFrame-objektet. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Hämtar textens horisontella justering. |
| [getTextOptions()](#getTextOptions--) | Hämtar textens alternativ. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Hämtar textens vertikala justering. |
| [getWidth()](#getWidth--) | Hämtar ramens bredd i enheter av 1/4000 av diagramområdet. |
| [getWidthPixel()](#getWidthPixel--) | Hämtar ramens bredd i enheter av pixel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Hämtar ramens bredd i enheter av förhållandet till diagramområdet. |
| [getX()](#getX--) | Hämtar X‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| [getXPixel()](#getXPixel--) | Hämtar x‑koordinaten för det övre vänstra hörnet i enheter av pixel. |
| [getXRatioToChart()](#getXRatioToChart--) | Hämtar x‑koordinaten för det övre vänstra hörnet i enheter av en bråkdel av diagramområdet. |
| [getY()](#getY--) | Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| [getYPixel()](#getYPixel--) | Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [getYRatioToChart()](#getYRatioToChart--) | Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av en bråkdel av diagramområdet. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Indikerar att texten är automatiskt genererad. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indikerar om diagramtexten roteras automatiskt. |
| [isAutomaticSize()](#isAutomaticSize--) | Indikerar om diagramramen har automatisk storlek. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indikerar om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är angiven. |
| [isDeleted()](#isDeleted--) | Indikerar om den här datamärket är raderad. |
| [isInnerMode()](#isInnerMode--) | Indikerar om storleken på plotområdet inkluderar tick-markeringar och axelrubriker. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Hämtar om en form ska anpassas automatiskt för att helt innehålla den beskrivna texten. |
| [isTextWrapped()](#isTextWrapped--) | Hämtar ett värde som indikerar om texten är radbruten. |
| [isVisible()](#isVisible--) | Representerar om titeln är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indikerar att texten är automatiskt genererad. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indikerar om diagramramen har automatisk storlek. |
| [setBackground(int value)](#setBackground-int-) | Ställer in bakgrundens visningsläge. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Ställer in bakgrundens visningsläge. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indikerar om den här datamärket är raderad. |
| [setDirectionType(int value)](#setDirectionType-int-) | Ställer in textens riktning. |
| [setHeight(int value)](#setHeight-int-) | Ställer in ramens höjd i enheter av 1/4000 av diagramområdet. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Ställer in ramens höjd i enheter av pixlar. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Ställer in ramens höjd i enheter av förhållandet till diagramområdet. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indikerar om storleken på plotområdet inkluderar tick-markeringar och axelrubriker. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Ställer in en referens till kalkylbladet. |
| [setOverLay(boolean value)](#setOverLay-boolean-) | Representerar en överlagrad centrerad titel på ett diagram utan att ändra diagrammets storlek. |
| [setPositionAuto()](#setPositionAuto--) | Ställ in ramens position till automatisk |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Representerar textens läsriktning. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Ställer in om en form ska anpassas automatiskt för att helt innehålla den beskrivna texten. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Representerar textens rotationsvinkel. |
| [setShadow(boolean value)](#setShadow-boolean-) | Sant om ramen har en skugga. |
| [setText(String value)](#setText-java.lang.String-) | Ställer in texten för enhetsetiketten. |
| [setTextDirection(int value)](#setTextDirection-int-) | Representerar textens läsriktning. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Ställer in textens horisontella justering. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Ställer in textens vertikala justering. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Ställer in ett värde som indikerar om texten är radbruten. |
| [setVisible(boolean value)](#setVisible-boolean-) | Representerar om titeln är synlig. |
| [setWidth(int value)](#setWidth-int-) | Ställer in bredden på ramen i enheter av 1/4000 av diagramområdet. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Ställer in bredden på ramen i enheter av pixel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Ställer in bredden på ramen i enheter av förhållandet till diagramområdet. |
| [setX(int value)](#setX-int-) | Ställer in X-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| [setXPixel(int value)](#setXPixel-int-) | Ställer in x-koordinaten för det övre vänstra hörnet i enheter av pixel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Ställer in x-koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. |
| [setY(int value)](#setY-int-) | Ställer in y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| [setYPixel(int value)](#setYPixel-int-) | Ställer in y-koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Ställer in y-koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters() {#characters--}
```
public FontSetting[] characters()
```


Hämtar rik textformatering för denna Titel.

**Returns:**
com.aspose.cells.FontSetting[] - returnerar FontSetting-array
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Returnerar ett Characters-objekt som representerar ett intervall av tecken inom texten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Indexet för tecknets början. |
| length | int | Antalet tecken. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Hämtar rik textformatering för denna Titel.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden Title.Characters(). Denna egenskap kommer att tas bort 12 månader senare sedan november 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
com.aspose.cells.FontSetting[] - returnerar FontSetting-array
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
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Hämtar textens riktning.

Se [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Hämtar ett [getFont()](../../com.aspose.cells/chartframe\#getFont--) objekt av det angivna ChartFrame-objektet.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Hämtar ramens höjd i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd ChartFrame.HeightRatioToChart‑egenskapen istället. Height = HeightRatioToChart \* 4000. Den här egenskapen kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Hämtar ramens höjd i enheter av förhållandet till diagramområdet.

**Remarks**

Detta är ett bråkvärde, dess giltiga intervall är mellan 0‑1. Hur konverterar man enheter av förhållande till pixlar? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Hämtar en referens till arbetsbladet.

**Returns:**
java.lang.String
### getOverLay() {#getOverLay--}
```
public boolean getOverLay()
```


Representerar en överlagrad centrerad titel på ett diagram utan att ändra diagrammets storlek.

**Returns:**
boolean
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Representerar textens läsriktning.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Representerar textens rotationsvinkel.

**Remarks**


0: Inte roterad.

255: Från topp till botten.

\-90: Nedåt.

90: Uppåt.


**Returns:**
int
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
### getText() {#getText--}
```
public String getText()
```


Hämtar texten för visningsenhetsetiketten.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Representerar textens läsriktning.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället ChartTextFrame.ReadingOrder‑egenskapen. Den här egenskapen kommer att tas bort 12 månader senare från och med mars 2020. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Hämtar ett [getFont()](../../com.aspose.cells/chartframe\#getFont--) objekt av det angivna ChartFrame-objektet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället ChartFrame.Font‑egenskapen. Den här egenskapen kommer att tas bort 12 månader senare från och med januari 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Hämtar textens horisontella justering.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Hämtar textens alternativ.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Hämtar textens vertikala justering.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Hämtar ramens bredd i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd ChartFrame.WidthRatioToChart‑egenskapen istället. Width = WidthRatioToChart \* 4000; Den här egenskapen kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Hämtar ramens bredd i enheter av förhållandet till diagramområdet.

**Remarks**

Detta är ett bråkvärde, dess giltiga intervall är mellan 0‑1. Hur konverterar man enheter av förhållande till pixlar? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Hämtar X‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd Title.XRatioToChart‑egenskapen istället. X = XRatioToChart \* 4000; Den här egenskapen kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Hämtar x‑koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. X i pixlar = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd Title.YRatioToChart‑egenskapen istället. Y = YRatioToChart \* 4000; Den här egenskapen kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. Y i pixlar = YRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoText() {#isAutoText--}
```
public boolean isAutoText()
```


Indikerar att texten är automatiskt genererad.

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Indikerar om diagramtexten roteras automatiskt.

**Returns:**
boolean
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
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indikerar om den här datamärket är raderad.

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
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


Hämtar om en form ska anpassas automatiskt för att helt innehålla den beskrivna texten. Automatisk anpassning innebär att texten i en form skalas för att rymma all text.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Hämtar ett värde som indikerar om texten är radbruten.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Representerar om titeln är synlig.

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

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


Indikerar att texten är automatiskt genererad.

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

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Indikerar om den här datamärket är raderad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Ställer in textens riktning.

Se [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Ställer in ramens höjd i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd ChartFrame.HeightRatioToChart‑egenskapen istället. Height = HeightRatioToChart \* 4000. Den här egenskapen kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Ställer in ramens höjd i enheter av förhållandet till diagramområdet.

**Remarks**

Detta är ett bråkvärde, dess giltiga intervall är mellan 0‑1. Hur konverterar man enheter av förhållande till pixlar? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

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

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


Ställer in en referens till kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOverLay(boolean value) {#setOverLay-boolean-}
```
public void setOverLay(boolean value)
```


Representerar en överlagrad centrerad titel på ett diagram utan att ändra diagrammets storlek.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Ställ in ramens position till automatisk

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Representerar textens läsriktning.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


Ställer in om en form ska anpassas automatiskt för att helt innehålla den beskrivna texten. Automatisk anpassning innebär att texten i en form skalas för att rymma all text.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Representerar textens rotationsvinkel.

**Remarks**


0: Inte roterad.

255: Från topp till botten.

\-90: Nedåt.

90: Uppåt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ställer in texten för enhetsetiketten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Representerar textens läsriktning.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället ChartTextFrame.ReadingOrder‑egenskapen. Den här egenskapen kommer att tas bort 12 månader senare från och med mars 2020. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Ställer in textens horisontella justering.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Ställer in textens vertikala justering.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Ställer in ett värde som indikerar om texten är radbruten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representerar om titeln är synlig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Ställer in bredden på ramen i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd ChartFrame.WidthRatioToChart‑egenskapen istället. Width = WidthRatioToChart \* 4000; Den här egenskapen kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Ställer in bredden på ramen i enheter av förhållandet till diagramområdet.

**Remarks**

Detta är ett bråkvärde, dess giltiga intervall är mellan 0‑1. Hur konverterar man enheter av förhållande till pixlar? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Ställer in X-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd Title.XRatioToChart‑egenskapen istället. X = XRatioToChart \* 4000; Den här egenskapen kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Ställer in x‑koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. X i pixlar = XRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Ställer in y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd Title.YRatioToChart‑egenskapen istället. Y = YRatioToChart \* 4000; Den här egenskapen kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Ställer in y‑koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. Y i pixlar = YRatioToChart \* Chart.ChartObject.Width;

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

