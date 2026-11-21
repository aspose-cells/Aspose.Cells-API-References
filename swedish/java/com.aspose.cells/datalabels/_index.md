---
title: "DataLabels"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av alla DataLabel‑objekt för den angivna serien."
type: docs
url: /sv/java/com.aspose.cells/datalabels/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class DataLabels extends ChartTextFrame
```

Inkapslar en samling av alla DataLabel‑objekt för den angivna serien.

**Example**

```
         //Set the DataLabels in the chart
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         DataLabels datalabels;
         for (int i = 0; i  <chart.getNSeries().getCount(); i++)
         {
             datalabels = chart.getNSeries().get(i).getDataLabels();
             //Set the position of DataLabels
             datalabels.setPosition(LabelPositionType.INSIDE_BASE);
             //Show the category name in the DataLabels
             datalabels.setShowCategoryName(true);
             //Show the value in the DataLabels
             datalabels.setShowValue(true);
             //Not show the percentage in the DataLabels
             datalabels.setShowPercentage(false);
             //Not show the legend key.
             datalabels.setShowLegendKey(false);
         }
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [applyFont()](#applyFont--) | Applicera teckensnittet för datamärkningarna på alla underordnade noder. |
| [characters(int startIndex, int length)](#characters-int-int-) | Returnerar ett Characters-objekt som representerar ett intervall av tecken inom texten. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Hämtar [getArea()](../../com.aspose.cells/datalabels\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. |
| [getBackground()](#getBackground--) | Hämtar bakgrundens visningsläge. |
| [getBackgroundMode()](#getBackgroundMode--) | Hämtar visningsläget för bakgrunden |
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
| [getDirectionType()](#getDirectionType--) | Hämtar textens riktning. |
| [getFont()](#getFont--) | Hämtar teckensnittet för DataLabels; |
| [getHeight()](#getHeight--) | Hämtar ramens höjd i enheter av 1/4000 av diagramområdet. |
| [getHeightPixel()](#getHeightPixel--) | Hämtar ramens höjd i enheter av pixlar. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Hämtar ramens höjd i enheter av förhållandet till diagramområdet. |
| [getLinkedSource()](#getLinkedSource--) | Hämtar en referens till arbetsbladet. |
| [getNumber()](#getNumber--) | Hämtar det inbyggda talformatet. |
| [getNumberFormat()](#getNumberFormat--) | Representerar formatsträngen för DataLabels-objektet. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna). |
| [getPosition()](#getPosition--) | Representerar positionen för datamärket. |
| [getReadingOrder()](#getReadingOrder--) | Representerar textens läsriktning. |
| [getRotationAngle()](#getRotationAngle--) | Representerar textens rotationsvinkel. |
| [getSeparatorType()](#getSeparatorType--) | Hämtar separator-typen som används för datamärkningarna i ett diagram. |
| [getSeparatorValue()](#getSeparatorValue--) | Hämtar separatorvärdet som används för datamärkningarna i ett diagram. |
| [getShadow()](#getShadow--) | Sant om ramen har en skugga. |
| [getShapeProperties()](#getShapeProperties--) | Hämtar [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) objektet. |
| [getShapeType()](#getShapeType--) | Hämtar formtypen för datamärket. |
| [getShowBubbleSize()](#getShowBubbleSize--) | Representerar ett specificerat diagrams datamärkesprocentvärdes visningsbeteende. |
| [getShowCategoryName()](#getShowCategoryName--) | Representerar ett specificerat diagrams datamärkes visning av kategorinamn. Sant för att visa kategorinamn för datamärkena i ett diagram. |
| [getShowCellRange()](#getShowCellRange--) | Indikerar om cellområdet ska visas som datamärken. |
| [getShowLegendKey()](#getShowLegendKey--) | Representerar ett specificerat diagrams datamärkes legendnyckels visningsbeteende. |
| [getShowPercentage()](#getShowPercentage--) | Representerar ett specificerat diagrams datamärkesprocentvärdes visningsbeteende. |
| [getShowSeriesName()](#getShowSeriesName--) | Indikerar om serienamnet visas på datamärkena i ett diagram. |
| [getShowValue()](#getShowValue--) | Representerar ett specificerat diagrams datamärkes värdevisningsbeteende. |
| [getText()](#getText--) | Hämtar texten för datamärket. |
| [getTextDirection()](#getTextDirection--) | Representerar textens läsriktning. |
| [getTextFont()](#getTextFont--) | Hämtar ett [getFont()](../../com.aspose.cells/chartframe\#getFont--) objekt av det angivna ChartFrame-objektet. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Hämtar textens horisontella justering. |
| [getTextOptions()](#getTextOptions--) | Hämtar textens alternativ. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Hämtar textens vertikala justering. |
| [getWidth()](#getWidth--) | Hämtar ramens bredd i enheter av 1/4000 av diagramområdet. |
| [getWidthPixel()](#getWidthPixel--) | Hämtar ramens bredd i enheter av pixel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Hämtar ramens bredd i enheter av förhållandet till diagramområdet. |
| [getX()](#getX--) | Hämtar x-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| [getXPixel()](#getXPixel--) | Hämtar x‑koordinaten för det övre vänstra hörnet i enheter av pixel. |
| [getXRatioToChart()](#getXRatioToChart--) | Hämtar x-koordinaten för det övre vänstra hörnet i enheter av förhållandet för diagramområdet. |
| [getY()](#getY--) | Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| [getYPixel()](#getYPixel--) | Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [getYRatioToChart()](#getYRatioToChart--) | Hämtar y-koordinaten för det övre vänstra hörnet i enheter av förhållandet för diagramområdet. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Indikerar att texten är automatiskt genererad. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indikerar om diagramtexten roteras automatiskt. |
| [isAutomaticSize()](#isAutomaticSize--) | Indikerar om diagramramen har automatisk storlek. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indikerar om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är angiven. |
| [isDeleted()](#isDeleted--) | Indikerar om den här datamärket är raderad. |
| [isInnerMode()](#isInnerMode--) | Indikerar om storleken på plotområdet inkluderar tick-markeringar och axelrubriker. |
| [isNeverOverlap()](#isNeverOverlap--) | Indikerar om Datalabels aldrig överlappar när ett pajdiagram omvandlas till en bild. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Hämtar om en form ska anpassas automatiskt för att helt innehålla den beskrivna texten. |
| [isTextWrapped()](#isTextWrapped--) | Hämtar ett värde som indikerar om texten är radbruten. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indikerar att texten är automatiskt genererad. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indikerar om diagramramen har automatisk storlek. |
| [setBackground(int value)](#setBackground-int-) | Ställer in bakgrundens visningsläge. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Ställer in visningsläget för bakgrunden |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indikerar om den här datamärket är raderad. |
| [setDirectionType(int value)](#setDirectionType-int-) | Ställer in textens riktning. |
| [setHeight(int value)](#setHeight-int-) | Ställer in ramens höjd i enheter av 1/4000 av diagramområdet. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Ställer in ramens höjd i enheter av pixlar. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Ställer in ramens höjd i enheter av förhållandet till diagramområdet. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indikerar om storleken på plotområdet inkluderar tick-markeringar och axelrubriker. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Ställer in en referens till kalkylbladet. |
| [setNeverOverlap(boolean value)](#setNeverOverlap-boolean-) | Indikerar om Datalabels aldrig överlappar när ett pajdiagram omvandlas till en bild. |
| [setNumber(int value)](#setNumber-int-) | Ställer in det inbyggda talformatet. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Representerar formatsträngen för DataLabels-objektet. |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna). |
| [setPosition(int value)](#setPosition-int-) | Representerar positionen för datamärket. |
| [setPositionAuto()](#setPositionAuto--) | Ställ in ramens position till automatisk |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Representerar textens läsriktning. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Ställer in om en form ska anpassas automatiskt för att helt innehålla den beskrivna texten. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Representerar textens rotationsvinkel. |
| [setSeparatorType(int value)](#setSeparatorType-int-) | Ställer in separator-typen som används för datamärkena i ett diagram. |
| [setSeparatorValue(String value)](#setSeparatorValue-java.lang.String-) | Ställer in separatorvärdet som används för dataetiketter på ett diagram. |
| [setShadow(boolean value)](#setShadow-boolean-) | Sant om ramen har en skugga. |
| [setShapeType(int value)](#setShapeType-int-) | Ställer in formtypen för dataetiketten. |
| [setShowBubbleSize(boolean value)](#setShowBubbleSize-boolean-) | Representerar ett specificerat diagrams datamärkesprocentvärdes visningsbeteende. |
| [setShowCategoryName(boolean value)](#setShowCategoryName-boolean-) | Representerar ett specificerat diagrams datamärkes visning av kategorinamn. Sant för att visa kategorinamn för datamärkena i ett diagram. |
| [setShowCellRange(boolean value)](#setShowCellRange-boolean-) | Indikerar om cellområdet ska visas som datamärken. |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Representerar ett specificerat diagrams datamärkes legendnyckels visningsbeteende. |
| [setShowPercentage(boolean value)](#setShowPercentage-boolean-) | Representerar ett specificerat diagrams datamärkesprocentvärdes visningsbeteende. |
| [setShowSeriesName(boolean value)](#setShowSeriesName-boolean-) | Indikerar om serienamnet visas på datamärkena i ett diagram. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Representerar ett specificerat diagrams datamärkes värdevisningsbeteende. |
| [setText(String value)](#setText-java.lang.String-) | Ställer in texten för dataetiketten. |
| [setTextDirection(int value)](#setTextDirection-int-) | Representerar textens läsriktning. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Ställer in textens horisontella justering. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Ställer in textens vertikala justering. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Ställer in ett värde som indikerar om texten är radbruten. |
| [setWidth(int value)](#setWidth-int-) | Ställer in bredden på ramen i enheter av 1/4000 av diagramområdet. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Ställer in bredden på ramen i enheter av pixel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Ställer in bredden på ramen i enheter av förhållandet till diagramområdet. |
| [setX(int value)](#setX-int-) | Ställer in x-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| [setXPixel(int value)](#setXPixel-int-) | Ställer in x-koordinaten för det övre vänstra hörnet i enheter av pixel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Ställer in x-koordinaten för det övre vänstra hörnet i enheter av förhållandet för diagramområdet. |
| [setY(int value)](#setY-int-) | Ställer in y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| [setYPixel(int value)](#setYPixel-int-) | Ställer in y-koordinaten för det övre vänstra hörnet i enheter av pixlar. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Ställer in y-koordinaten för det övre vänstra hörnet i enheter av förhållandet för diagramområdet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyFont() {#applyFont--}
```
public void applyFont()
```


Applicera teckensnittet för datamärkningarna på alla underordnade noder.

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


Hämtar [getArea()](../../com.aspose.cells/datalabels\#getArea--).

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


Hämtar visningsläget för bakgrunden

Se [BackgroundMode](../../com.aspose.cells/backgroundmode).

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


Hämtar teckensnittet för DataLabels;

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
### getNumber() {#getNumber--}
```
public int getNumber()
```


Hämtar det inbyggda talformatet.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Representerar formatsträngen för DataLabels-objektet.

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna).

**Returns:**
boolean
### getPosition() {#getPosition--}
```
public int getPosition()
```


Representerar positionen för datamärket.

Se [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Returns:**
int
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
### getSeparatorType() {#getSeparatorType--}
```
public int getSeparatorType()
```


Hämtar separator-typen som används för datamärkningarna i ett diagram.

Se [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

För att ange en anpassad separator, vänligen ställ in egenskapen [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) som [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) och ange sedan det förväntade värdet för [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Returns:**
int
### getSeparatorValue() {#getSeparatorValue--}
```
public String getSeparatorValue()
```


Hämtar separatorvärdet som används för datamärkningarna i ett diagram.

**Returns:**
java.lang.String
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
### getShapeType() {#getShapeType--}
```
public int getShapeType()
```


Hämtar formtypen för datamärket.

Se [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Returns:**
int
### getShowBubbleSize() {#getShowBubbleSize--}
```
public boolean getShowBubbleSize()
```


Representerar ett specificerat diagrammets dataetiketts procentvärdesvisningsbeteende. True visar procentvärdet. False döljer procentvärdet.

**Returns:**
boolean
### getShowCategoryName() {#getShowCategoryName--}
```
public boolean getShowCategoryName()
```


Representerar ett specificerat diagrammets dataetiketts kategorinamnsvisningsbeteende. True för att visa kategorinamnet för dataetiketterna på ett diagram. False för att dölja.

**Returns:**
boolean
### getShowCellRange() {#getShowCellRange--}
```
public boolean getShowCellRange()
```


Indikerar om cellområdet ska visas som datamärken.

**Returns:**
boolean
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Representerar ett specificerat diagrammets dataetiketts legendnyckelvisningsbeteende. True om legendnyckeln för dataetiketten är synlig.

**Returns:**
boolean
### getShowPercentage() {#getShowPercentage--}
```
public boolean getShowPercentage()
```


Representerar ett specificerat diagrammets dataetiketts procentvärdesvisningsbeteende. True visar procentvärdet. False för att dölja.

**Returns:**
boolean
### getShowSeriesName() {#getShowSeriesName--}
```
public boolean getShowSeriesName()
```


Indikerar om serienamnet visas på dataetiketterna i ett diagram. True för att visa serienamnet. False för att dölja.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Representerar ett specificerat diagrammets dataetiketts värdevisningsbeteende. True visar värdena. False för att dölja.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Hämtar texten för datamärket.

**Remarks**

Fungerar endast när detta är en dataetikett för en diagrampunkt.

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


Hämtar x-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.XRatioToChart. X = XRatioToChart \\* 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Hämtar x-koordinaten för det övre vänstra hörnet i enheter av förhållandet för diagramområdet.

**Remarks**

Detta är ett bråkvärde, dess giltiga intervall är mellan 0-1. Hur konverterar man enheter av förhållande till pixlar? XPixel = XRatioToChart \\* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.YRatioToChart. Y = YRatioToChart \\* 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Hämtar y-koordinaten för det övre vänstra hörnet i enheter av förhållandet för diagramområdet.

**Remarks**

Detta är ett bråkvärde, dess giltiga intervall är mellan 0-1. Hur konverterar man enheter av förhållande till pixlar? YPixel = YRatioToChart \\* Chart.ChartObject.Height;

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
### isNeverOverlap() {#isNeverOverlap--}
```
public boolean isNeverOverlap()
```


Indikerar om dataetiketter aldrig överlappar när en pajdiagram konverteras till bild. Obs: den här egenskapen är endast meningsfull när en pajdiagram konverteras till bild.

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


Ställer in visningsläget för bakgrunden

Se [BackgroundMode](../../com.aspose.cells/backgroundmode).

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

### setNeverOverlap(boolean value) {#setNeverOverlap-boolean-}
```
public void setNeverOverlap(boolean value)
```


Indikerar om dataetiketter aldrig överlappar när en pajdiagram konverteras till bild. Obs: den här egenskapen är endast meningsfull när en pajdiagram konverteras till bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Ställer in det inbyggda talformatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Representerar formatsträngen för DataLabels-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Representerar positionen för datamärket.

Se [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setSeparatorType(int value) {#setSeparatorType-int-}
```
public void setSeparatorType(int value)
```


Ställer in separator-typen som används för datamärkena i ett diagram.

Se [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

För att ange en anpassad separator, vänligen ställ in egenskapen [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) som [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) och ange sedan det förväntade värdet för [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSeparatorValue(String value) {#setSeparatorValue-java.lang.String-}
```
public void setSeparatorValue(String value)
```


Ställer in separatorvärdet som används för dataetiketter på ett diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

### setShapeType(int value) {#setShapeType-int-}
```
public void setShapeType(int value)
```


Ställer in formtypen för dataetiketten.

Se [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShowBubbleSize(boolean value) {#setShowBubbleSize-boolean-}
```
public void setShowBubbleSize(boolean value)
```


Representerar ett specificerat diagrammets dataetiketts procentvärdesvisningsbeteende. True visar procentvärdet. False döljer procentvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowCategoryName(boolean value) {#setShowCategoryName-boolean-}
```
public void setShowCategoryName(boolean value)
```


Representerar ett specificerat diagrammets dataetiketts kategorinamnsvisningsbeteende. True för att visa kategorinamnet för dataetiketterna på ett diagram. False för att dölja.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowCellRange(boolean value) {#setShowCellRange-boolean-}
```
public void setShowCellRange(boolean value)
```


Indikerar om cellområdet ska visas som datamärken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Representerar ett specificerat diagrammets dataetiketts legendnyckelvisningsbeteende. True om legendnyckeln för dataetiketten är synlig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowPercentage(boolean value) {#setShowPercentage-boolean-}
```
public void setShowPercentage(boolean value)
```


Representerar ett specificerat diagrammets dataetiketts procentvärdesvisningsbeteende. True visar procentvärdet. False för att dölja.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowSeriesName(boolean value) {#setShowSeriesName-boolean-}
```
public void setShowSeriesName(boolean value)
```


Indikerar om serienamnet visas på dataetiketterna i ett diagram. True för att visa serienamnet. False för att dölja.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Representerar ett specificerat diagrammets dataetiketts värdevisningsbeteende. True visar värdena. False för att dölja.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ställer in texten för dataetiketten.

**Remarks**

Fungerar endast när detta är en dataetikett för en diagrampunkt.

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


Ställer in x-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.XRatioToChart. X = XRatioToChart \\* 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Ställer in x-koordinaten för det övre vänstra hörnet i enheter av förhållandet för diagramområdet.

**Remarks**

Detta är ett bråkvärde, dess giltiga intervall är mellan 0-1. Hur konverterar man enheter av förhållande till pixlar? XPixel = XRatioToChart \\* Chart.ChartObject.Width;

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

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.YRatioToChart. Y = YRatioToChart \\* 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Ställer in y-koordinaten för det övre vänstra hörnet i enheter av förhållandet för diagramområdet.

**Remarks**

Detta är ett bråkvärde, dess giltiga intervall är mellan 0-1. Hur konverterar man enheter av förhållande till pixlar? YPixel = YRatioToChart \\* Chart.ChartObject.Height;

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

