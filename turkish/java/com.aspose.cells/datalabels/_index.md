---
title: "DataLabels"
second_title: "Aspose.Cells for Java API Referansı"
description: "Belirtilen Seriye ait tüm DataLabel nesnelerinin bir koleksiyonunu kapsüller."
type: docs
url: /tr/java/com.aspose.cells/datalabels/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class DataLabels extends ChartTextFrame
```

Belirtilen Seriye ait tüm DataLabel nesnelerinin bir koleksiyonunu kapsüller.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [applyFont()](#applyFont--) | Veri etiketlerinin yazı tipini tüm alt düğümlere uygula. |
| [characters(int startIndex, int length)](#characters-int-int-) | Metin içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Alır [getArea()](../../com.aspose.cells/datalabels\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. |
| [getBackground()](#getBackground--) | Arka planın görüntüleme modunu alır. |
| [getBackgroundMode()](#getBackgroundMode--) | Arka planın görüntüleme modunu alır |
| [getBorder()](#getBorder--) | Alır [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Bu nesnenin ait olduğu grafiği alır. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Grafik alanının 1/4000 biriminde varsayılan konumun yüksekliğini temsil eder. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | Grafik alanının kesir biriminde varsayılan konumun yüksekliğini temsil eder. |
| [getDefaultWidth()](#getDefaultWidth--) | Grafik alanının 1/4000 biriminde varsayılan konumun genişliğini temsil eder. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | Grafik alanının Kesir biriminde varsayılan konumun genişliğini temsil eder. |
| [getDefaultX()](#getDefaultX--) | Grafik alanının 1/4000 biriminde varsayılan konumun x değerini temsil eder. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | Grafik alanının Kesir biriminde varsayılan konumun x değerini temsil eder. |
| [getDefaultY()](#getDefaultY--) | Grafik alanının 1/4000 biriminde varsayılan konumun y değerini temsil eder. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | Grafik alanının kesir biriminde varsayılan konumun y değerini temsil eder. |
| [getDirectionType()](#getDirectionType--) | Metnin yönünü alır. |
| [getFont()](#getFont--) | Alır DataLabels'ın yazı tipini; |
| [getHeight()](#getHeight--) | Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini alır. |
| [getHeightPixel()](#getHeightPixel--) | Çerçevenin yüksekliğini piksel biriminde alır. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Grafik alanının oran biriminde çerçevenin yüksekliğini alır. |
| [getLinkedSource()](#getLinkedSource--) | Çalışma sayfasına bir referans alır. |
| [getNumber()](#getNumber--) | Alır yerleşik sayı biçimini. |
| [getNumberFormat()](#getNumberFormat--) | DataLabels nesnesi için biçim dizesini temsil eder. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | Sayı biçimi hücrelere bağlıysa doğru (bu sayede hücrelerde değiştiğinde etiketlerdeki sayı biçimi de değişir). |
| [getPosition()](#getPosition--) | Veri etiketinin konumunu temsil eder. |
| [getReadingOrder()](#getReadingOrder--) | Metin okuma sırasını temsil eder. |
| [getRotationAngle()](#getRotationAngle--) | Metin döndürme açısını temsil eder. |
| [getSeparatorType()](#getSeparatorType--) | Alır bir grafikte veri etiketleri için kullanılan ayırıcı tipini. |
| [getSeparatorValue()](#getSeparatorValue--) | Alır bir grafikte veri etiketleri için kullanılan ayırıcı değerini. |
| [getShadow()](#getShadow--) | Çerçevenin gölgesi varsa doğru. |
| [getShapeProperties()](#getShapeProperties--) | [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) nesnesini alır. |
| [getShapeType()](#getShapeType--) | Alır veri etiketinin şekil tipini. |
| [getShowBubbleSize()](#getShowBubbleSize--) | Belirtilen grafiğin veri etiketi yüzde değeri gösterim davranışını temsil eder. |
| [getShowCategoryName()](#getShowCategoryName--) | Belirtilen grafiğin veri etiketi kategori adı gösterim davranışını temsil eder. Grafikte veri etiketleri için kategori adını göstermek true. |
| [getShowCellRange()](#getShowCellRange--) | Hücre aralığını veri etiketi olarak gösterip göstermeyeceğini belirtir. |
| [getShowLegendKey()](#getShowLegendKey--) | Belirtilen grafiğin veri etiketi lejand anahtarı gösterim davranışını temsil eder. |
| [getShowPercentage()](#getShowPercentage--) | Belirtilen grafiğin veri etiketi yüzde değeri gösterim davranışını temsil eder. |
| [getShowSeriesName()](#getShowSeriesName--) | Seri adının bir grafikte veri etiketlerinde gösterilip gösterilmeyeceğini belirtir. |
| [getShowValue()](#getShowValue--) | Belirtilen grafiğin veri etiketi değerleri gösterim davranışını temsil eder. |
| [getText()](#getText--) | Alır veri etiketinin metnini. |
| [getTextDirection()](#getTextDirection--) | Metin okuma sırasını temsil eder. |
| [getTextFont()](#getTextFont--) | Belirtilen ChartFrame nesnesinin bir [getFont()](../../com.aspose.cells/chartframe\#getFont--) nesnesini alır. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Metnin yatay hizalamasını alır. |
| [getTextOptions()](#getTextOptions--) | Metnin seçeneklerini alır. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Metnin dikey hizalamasını alır. |
| [getWidth()](#getWidth--) | Grafik alanının 1/4000 biriminde çerçevenin genişliğini alır. |
| [getWidthPixel()](#getWidthPixel--) | Çerçevenin genişliğini piksel biriminde alır. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Grafik alanının oran biriminde çerçevenin genişliğini alır. |
| [getX()](#getX--) | Grafik alanının sol üst köşesinin x koordinatını 1/4000 biriminde alır. |
| [getXPixel()](#getXPixel--) | Sol üst köşenin x koordinatını piksel biriminde alır. |
| [getXRatioToChart()](#getXRatioToChart--) | Grafik alanının sol üst köşesinin x koordinatını oran biriminde alır. |
| [getY()](#getY--) | Grafik alanının 1/4000 biriminde sol üst köşenin y koordinatını alır. |
| [getYPixel()](#getYPixel--) | Piksel biriminde sol üst köşenin y koordinatını alır. |
| [getYRatioToChart()](#getYRatioToChart--) | Grafik alanının sol üst köşesinin y koordinatını oran biriminde alır. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Grafiğin metninin otomatik olarak döndürülüp döndürülmediğini gösterir. |
| [isAutomaticSize()](#isAutomaticSize--) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir. |
| [isDeleted()](#isDeleted--) | Bu veri etiketinin silinip silinmediğini gösterir. |
| [isInnerMode()](#isInnerMode--) | Çizim alanı boyutunun işaretçileri ve eksen etiketlerini içerip içermediğini gösterir. |
| [isNeverOverlap()](#isNeverOverlap--) | Pasta grafiğini görüntüye dönüştürürken Datalabels'in hiç çakışmamasını belirtir. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Bir şeklin içinde tanımlanan metni tamamen içerecek şekilde otomatik sığdırılıp sığdırılmayacağını alır. |
| [isTextWrapped()](#isTextWrapped--) | Metnin kaydırılıp kaydırılmadığını gösteren bir değeri alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [setBackground(int value)](#setBackground-int-) | Arka planın görüntüleme modunu ayarlar. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Arka planın görüntüleme modunu ayarlar |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Bu veri etiketinin silinip silinmediğini gösterir. |
| [setDirectionType(int value)](#setDirectionType-int-) | Metnin yönünü ayarlar. |
| [setHeight(int value)](#setHeight-int-) | Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini ayarlar. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Piksel biriminde çerçevenin yüksekliğini ayarlar. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Grafik alanının oran biriminde çerçevenin yüksekliğini ayarlar. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Çizim alanı boyutunun işaretçileri ve eksen etiketlerini içerip içermediğini gösterir. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Çalışma sayfasına bir referans ayarlar. |
| [setNeverOverlap(boolean value)](#setNeverOverlap-boolean-) | Pasta grafiğini görüntüye dönüştürürken Datalabels'in hiç çakışmamasını belirtir. |
| [setNumber(int value)](#setNumber-int-) | Ayarlıyor yerleşik sayı biçimini. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | DataLabels nesnesi için biçim dizesini temsil eder. |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | Sayı biçimi hücrelere bağlıysa doğru (bu sayede hücrelerde değiştiğinde etiketlerdeki sayı biçimi de değişir). |
| [setPosition(int value)](#setPosition-int-) | Veri etiketinin konumunu temsil eder. |
| [setPositionAuto()](#setPositionAuto--) | Çerçevenin konumunu otomatik olarak ayarla |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Metin okuma sırasını temsil eder. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Bir şeklin içinde tanımlanan metni tamamen içerecek şekilde otomatik sığdırılıp sığdırılmayacağını ayarlar. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Metin döndürme açısını temsil eder. |
| [setSeparatorType(int value)](#setSeparatorType-int-) | Ayarlıyor bir grafikte veri etiketleri için kullanılan ayırıcı tipini. |
| [setSeparatorValue(String value)](#setSeparatorValue-java.lang.String-) | Ayarlıyor bir grafikte veri etiketleri için kullanılan ayırıcı değerini. |
| [setShadow(boolean value)](#setShadow-boolean-) | Çerçevenin gölgesi varsa doğru. |
| [setShapeType(int value)](#setShapeType-int-) | Ayarlıyor veri etiketinin şekil tipini. |
| [setShowBubbleSize(boolean value)](#setShowBubbleSize-boolean-) | Belirtilen grafiğin veri etiketi yüzde değeri gösterim davranışını temsil eder. |
| [setShowCategoryName(boolean value)](#setShowCategoryName-boolean-) | Belirtilen grafiğin veri etiketi kategori adı gösterim davranışını temsil eder. Grafikte veri etiketleri için kategori adını göstermek true. |
| [setShowCellRange(boolean value)](#setShowCellRange-boolean-) | Hücre aralığını veri etiketi olarak gösterip göstermeyeceğini belirtir. |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Belirtilen grafiğin veri etiketi lejand anahtarı gösterim davranışını temsil eder. |
| [setShowPercentage(boolean value)](#setShowPercentage-boolean-) | Belirtilen grafiğin veri etiketi yüzde değeri gösterim davranışını temsil eder. |
| [setShowSeriesName(boolean value)](#setShowSeriesName-boolean-) | Seri adının bir grafikte veri etiketlerinde gösterilip gösterilmeyeceğini belirtir. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Belirtilen grafiğin veri etiketi değerleri gösterim davranışını temsil eder. |
| [setText(String value)](#setText-java.lang.String-) | Ayarlıyor veri etiketinin metnini. |
| [setTextDirection(int value)](#setTextDirection-int-) | Metin okuma sırasını temsil eder. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Metnin yatay hizalamasını ayarlar. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Metnin dikey hizalamasını ayarlar. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Metnin kaydırılıp kaydırılmadığını gösteren bir değeri ayarlar. |
| [setWidth(int value)](#setWidth-int-) | Çerçevenin genişliğini, grafik alanının 1/4000'i biriminde ayarlar. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Çerçevenin genişliğini piksel biriminde ayarlar. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Çerçevenin genişliğini, grafik alanının oranı biriminde ayarlar. |
| [setX(int value)](#setX-int-) | Grafik alanının sol üst köşesinin x koordinatını 1/4000 biriminde ayarlar. |
| [setXPixel(int value)](#setXPixel-int-) | Üst sol köşenin x koordinatını piksel biriminde ayarlar. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Grafik alanının sol üst köşesinin x koordinatını oran biriminde ayarlar. |
| [setY(int value)](#setY-int-) | Üst sol köşenin y koordinatını, grafik alanının 1/4000'i biriminde ayarlar. |
| [setYPixel(int value)](#setYPixel-int-) | Üst sol köşenin y koordinatını piksel biriminde ayarlar. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Grafik alanının sol üst köşesinin y koordinatını oran biriminde ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyFont() {#applyFont--}
```
public void applyFont()
```


Veri etiketlerinin yazı tipini tüm alt düğümlere uygula.

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Metin içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Karakterin başlangıç indeksi. |
| length | int | Karakter sayısı. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArea() {#getArea--}
```
public Area getArea()
```


Alır [getArea()](../../com.aspose.cells/datalabels\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. Varsayılan değer Doğru.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


Arka planın görüntüleme modunu alır. Bu özellik yalnızca Excel 2003 ve önceki sürümlerde geçerlidir.

Bakınız [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.Area.FillFormat.FillType** özelliğini kullanın. Örneğin, BackgroundMode'u Opaque olarak ayarlamanız gerekiyorsa, aşağıdaki kodu kullanabilirsiniz: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Bu özellik, OCAK 2012'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Arka planın görüntüleme modunu alır

Bakınız [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Alır [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


Bu nesnenin ait olduğu grafiği alır.

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


Grafik alanının 1/4000 biriminde varsayılan konumun yüksekliğini temsil eder.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.DefaultHeightRatioToChart** özelliğini kullanın. DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); Bu özellik, ŞUBAT 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


Grafik alanının kesir biriminde varsayılan konumun yüksekliğini temsil eder.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Grafik alanının 1/4000 biriminde varsayılan konumun genişliğini temsil eder.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.DefaultWidthRatioToChart** özelliğini kullanın. DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); Bu özellik, ŞUBAT 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


Grafik alanının Kesir biriminde varsayılan konumun genişliğini temsil eder.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Grafik alanının 1/4000 biriminde varsayılan konumun x değerini temsil eder.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.DefaultXRatioToChart** özelliğini kullanın. DefaultX = (int)(DefaultXRatioToChart \* 4000); Bu özellik, ŞUBAT 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


Grafik alanının Kesir biriminde varsayılan konumun x değerini temsil eder.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Grafik alanının 1/4000 biriminde varsayılan konumun y değerini temsil eder.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.DefaultYRatioToChart** özelliğini kullanın. DefaultY = (int)(DefaultYRatioToChart \* 4000); Bu özellik, ŞUBAT 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


Grafik alanının kesir biriminde varsayılan konumun y değerini temsil eder.

**Returns:**
double
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Metnin yönünü alır.

Bakınız [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Alır DataLabels'ın yazı tipini;

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.HeightRatioToChart** özelliğini kullanın. Height = HeightRatioToChart \* 4000. Bu özellik, ŞUBAT 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Çerçevenin yüksekliğini piksel biriminde alır.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


Grafik alanının oran biriminde çerçevenin yüksekliğini alır.

**Remarks**

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksele nasıl dönüştürülür? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Çalışma sayfasına bir referans alır.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Alır yerleşik sayı biçimini.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


DataLabels nesnesi için biçim dizesini temsil eder.

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


Sayı biçimi hücrelere bağlıysa doğru (bu sayede hücrelerde değiştiğinde etiketlerdeki sayı biçimi de değişir).

**Returns:**
boolean
### getPosition() {#getPosition--}
```
public int getPosition()
```


Veri etiketinin konumunu temsil eder.

Bakınız [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Metin okuma sırasını temsil eder.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Metin döndürme açısını temsil eder.

**Remarks**


0: Döndürülmemiş.

255: Yukarıdan Aşağıya.

\-90: Aşağı.

90: Yukarı.


**Returns:**
int
### getSeparatorType() {#getSeparatorType--}
```
public int getSeparatorType()
```


Alır bir grafikte veri etiketleri için kullanılan ayırıcı tipini.

Bakınız [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

Özel ayırıcıyı ayarlamak için, lütfen [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) özelliğini [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) olarak ayarlayın ve ardından [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--) için beklenen değeri belirtin.

**Returns:**
int
### getSeparatorValue() {#getSeparatorValue--}
```
public String getSeparatorValue()
```


Alır bir grafikte veri etiketleri için kullanılan ayırıcı değerini.

**Returns:**
java.lang.String
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Çerçevenin gölgesi varsa doğru.

**Remarks**

Yalnızca xls dosyasındaki grafikler için.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


[getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) nesnesini alır.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeType() {#getShapeType--}
```
public int getShapeType()
```


Alır veri etiketinin şekil tipini.

Bakınız [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Returns:**
int
### getShowBubbleSize() {#getShowBubbleSize--}
```
public boolean getShowBubbleSize()
```


Belirli bir grafiğin veri etiketi yüzde değeri görüntüleme davranışını temsil eder. True yüzde değerini gösterir. False yüzde değerini gizler.

**Returns:**
boolean
### getShowCategoryName() {#getShowCategoryName--}
```
public boolean getShowCategoryName()
```


Belirli bir grafiğin veri etiketi kategori adı görüntüleme davranışını temsil eder. True, grafikteki veri etiketleri için kategori adını gösterir. False, gizler.

**Returns:**
boolean
### getShowCellRange() {#getShowCellRange--}
```
public boolean getShowCellRange()
```


Hücre aralığını veri etiketi olarak gösterip göstermeyeceğini belirtir.

**Returns:**
boolean
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Belirli bir grafiğin veri etiketi lejand anahtarı görüntüleme davranışını temsil eder. True, veri etiketi lejand anahtarı görünürse.

**Returns:**
boolean
### getShowPercentage() {#getShowPercentage--}
```
public boolean getShowPercentage()
```


Belirli bir grafiğin veri etiketi yüzde değeri görüntüleme davranışını temsil eder. True yüzde değerini gösterir. False gizler.

**Returns:**
boolean
### getShowSeriesName() {#getShowSeriesName--}
```
public boolean getShowSeriesName()
```


Bir grafikteki veri etiketlerinde seri adının gösterilip gösterilmediğini belirtir. True, seri adını gösterir. False, gizler.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Belirli bir grafiğin veri etiketi değerleri görüntüleme davranışını temsil eder. True değerleri gösterir. False gizler.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Alır veri etiketinin metnini.

**Remarks**

Yalnızca bu bir grafik noktasının veri etiketi olduğunda çalışır.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Metin okuma sırasını temsil eder.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ChartTextFrame.ReadingOrder özelliğini kullanın. Bu özellik, Mart 2020'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Belirtilen ChartFrame nesnesinin bir [getFont()](../../com.aspose.cells/chartframe\#getFont--) nesnesini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ChartFrame.Font özelliğini kullanın. Bu özellik, OCAK 2012'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Metnin yatay hizalamasını alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Metnin seçeneklerini alır.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Metnin dikey hizalamasını alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Grafik alanının 1/4000 biriminde çerçevenin genişliğini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ChartFrame.WidthRatioToChart özelliğini kullanın. Width = WidthRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Çerçevenin genişliğini piksel biriminde alır.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


Grafik alanının oran biriminde çerçevenin genişliğini alır.

**Remarks**

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksellere nasıl dönüştürülür? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Grafik alanının sol üst köşesinin x koordinatını 1/4000 biriminde alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine ChartFrame.XRatioToChart özelliğini kullanın. X = XRatioToChart \* 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Sol üst köşenin x koordinatını piksel biriminde alır.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


Grafik alanının sol üst köşesinin x koordinatını oran biriminde alır.

**Remarks**

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksellere nasıl dönüştürürsünüz? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Grafik alanının 1/4000 biriminde sol üst köşenin y koordinatını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine ChartFrame.YRatioToChart özelliğini kullanın. Y = YRatioToChart \* 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Piksel biriminde sol üst köşenin y koordinatını alır.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


Grafik alanının sol üst köşesinin y koordinatını oran biriminde alır.

**Remarks**

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksellere nasıl dönüştürürsünüz? YPixel = YRatioToChart \* Chart.ChartObject.Height;

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


Metnin otomatik olarak oluşturulduğunu gösterir.

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Grafiğin metninin otomatik olarak döndürülüp döndürülmediğini gösterir.

**Returns:**
boolean
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir.

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Bu veri etiketinin silinip silinmediğini gösterir.

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Çizim alanının boyutunun tik işaretlerini ve eksen etiketlerini içerip içermediğini gösterir. False, boyutun çizim alanının, tik işaretlerinin ve eksen etiketlerinin boyutunu belirleyeceğini belirtir.

**Remarks**

Yalnızca Xlsx dosyası için.

**Returns:**
boolean
### isNeverOverlap() {#isNeverOverlap--}
```
public boolean isNeverOverlap()
```


Datalabels'in Pasta Grafiği görüntüye dönüştürürken hiç çakışıp çakışmadığını belirtir. Not: bu özellik yalnızca bir Pasta Grafiği görüntüye dönüştürülürken anlamlıdır.

**Returns:**
boolean
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


Bir şeklin içindeki metni tamamen kapsayacak şekilde otomatik olarak sığdırılıp sığdırılmayacağını alır. Otomatik sığdırma, şekil içindeki metnin tüm metni içerecek şekilde ölçeklendirilmesidir.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Metnin kaydırılıp kaydırılmadığını gösteren bir değeri alır.

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


Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. Varsayılan değer Doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


Metnin otomatik olarak oluşturulduğunu gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


Arka planın görüntüleme modunu ayarlar. Bu özellik yalnızca Excel 2003 ve daha önceki sürümlerde geçerlidir.

Bakınız [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.Area.FillFormat.FillType** özelliğini kullanın. Örneğin, BackgroundMode'u Opaque olarak ayarlamanız gerekiyorsa, aşağıdaki kodu kullanabilirsiniz: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Bu özellik, OCAK 2012'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Arka planın görüntüleme modunu ayarlar

Bakınız [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Bu veri etiketinin silinip silinmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Metnin yönünü ayarlar.

Bakınız [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.HeightRatioToChart** özelliğini kullanın. Height = HeightRatioToChart \* 4000. Bu özellik, ŞUBAT 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Piksel biriminde çerçevenin yüksekliğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


Grafik alanının oran biriminde çerçevenin yüksekliğini ayarlar.

**Remarks**

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksele nasıl dönüştürülür? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Çizim alanının boyutunun tik işaretlerini ve eksen etiketlerini içerip içermediğini gösterir. False, boyutun çizim alanının, tik işaretlerinin ve eksen etiketlerinin boyutunu belirleyeceğini belirtir.

**Remarks**

Yalnızca Xlsx dosyası için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


Çalışma sayfasına bir referans ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNeverOverlap(boolean value) {#setNeverOverlap-boolean-}
```
public void setNeverOverlap(boolean value)
```


Datalabels'in Pasta Grafiği görüntüye dönüştürürken hiç çakışıp çakışmadığını belirtir. Not: bu özellik yalnızca bir Pasta Grafiği görüntüye dönüştürülürken anlamlıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Ayarlıyor yerleşik sayı biçimini.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


DataLabels nesnesi için biçim dizesini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


Sayı biçimi hücrelere bağlıysa doğru (bu sayede hücrelerde değiştiğinde etiketlerdeki sayı biçimi de değişir).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Veri etiketinin konumunu temsil eder.

Bakınız [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Çerçevenin konumunu otomatik olarak ayarla

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Metin okuma sırasını temsil eder.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


Bir şeklin içindeki metni tamamen kapsayacak şekilde otomatik olarak sığdırılıp sığdırılmayacağını ayarlar. Otomatik sığdırma, şekil içindeki metnin tüm metni içerecek şekilde ölçeklendirilmesidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Metin döndürme açısını temsil eder.

**Remarks**


0: Döndürülmemiş.

255: Yukarıdan Aşağıya.

\-90: Aşağı.

90: Yukarı.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSeparatorType(int value) {#setSeparatorType-int-}
```
public void setSeparatorType(int value)
```


Ayarlıyor bir grafikte veri etiketleri için kullanılan ayırıcı tipini.

Bakınız [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

Özel ayırıcıyı ayarlamak için, lütfen [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) özelliğini [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) olarak ayarlayın ve ardından [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--) için beklenen değeri belirtin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSeparatorValue(String value) {#setSeparatorValue-java.lang.String-}
```
public void setSeparatorValue(String value)
```


Ayarlıyor bir grafikte veri etiketleri için kullanılan ayırıcı değerini.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Çerçevenin gölgesi varsa doğru.

**Remarks**

Yalnızca xls dosyasındaki grafikler için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShapeType(int value) {#setShapeType-int-}
```
public void setShapeType(int value)
```


Ayarlıyor veri etiketinin şekil tipini.

Bakınız [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShowBubbleSize(boolean value) {#setShowBubbleSize-boolean-}
```
public void setShowBubbleSize(boolean value)
```


Belirli bir grafiğin veri etiketi yüzde değeri görüntüleme davranışını temsil eder. True yüzde değerini gösterir. False yüzde değerini gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowCategoryName(boolean value) {#setShowCategoryName-boolean-}
```
public void setShowCategoryName(boolean value)
```


Belirli bir grafiğin veri etiketi kategori adı görüntüleme davranışını temsil eder. True, grafikteki veri etiketleri için kategori adını gösterir. False, gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowCellRange(boolean value) {#setShowCellRange-boolean-}
```
public void setShowCellRange(boolean value)
```


Hücre aralığını veri etiketi olarak gösterip göstermeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Belirli bir grafiğin veri etiketi lejand anahtarı görüntüleme davranışını temsil eder. True, veri etiketi lejand anahtarı görünürse.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowPercentage(boolean value) {#setShowPercentage-boolean-}
```
public void setShowPercentage(boolean value)
```


Belirli bir grafiğin veri etiketi yüzde değeri görüntüleme davranışını temsil eder. True yüzde değerini gösterir. False gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowSeriesName(boolean value) {#setShowSeriesName-boolean-}
```
public void setShowSeriesName(boolean value)
```


Bir grafikteki veri etiketlerinde seri adının gösterilip gösterilmediğini belirtir. True, seri adını gösterir. False, gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Belirli bir grafiğin veri etiketi değerleri görüntüleme davranışını temsil eder. True değerleri gösterir. False gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ayarlıyor veri etiketinin metnini.

**Remarks**

Yalnızca bu bir grafik noktasının veri etiketi olduğunda çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Metin okuma sırasını temsil eder.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ChartTextFrame.ReadingOrder özelliğini kullanın. Bu özellik, Mart 2020'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Metnin yatay hizalamasını ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Metnin dikey hizalamasını ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Metnin kaydırılıp kaydırılmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Çerçevenin genişliğini, grafik alanının 1/4000'i biriminde ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ChartFrame.WidthRatioToChart özelliğini kullanın. Width = WidthRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Çerçevenin genişliğini piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


Çerçevenin genişliğini, grafik alanının oranı biriminde ayarlar.

**Remarks**

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksellere nasıl dönüştürülür? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Grafik alanının sol üst köşesinin x koordinatını 1/4000 biriminde ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine ChartFrame.XRatioToChart özelliğini kullanın. X = XRatioToChart \* 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Üst sol köşenin x koordinatını piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


Grafik alanının sol üst köşesinin x koordinatını oran biriminde ayarlar.

**Remarks**

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksellere nasıl dönüştürürsünüz? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Üst sol köşenin y koordinatını, grafik alanının 1/4000'i biriminde ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine ChartFrame.YRatioToChart özelliğini kullanın. Y = YRatioToChart \* 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Üst sol köşenin y koordinatını piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


Grafik alanının sol üst köşesinin y koordinatını oran biriminde ayarlar.

**Remarks**

Bu bir kesir değeridir, geçerli aralığı 0-1 arasındadır. Oran birimlerini piksellere nasıl dönüştürürsünüz? YPixel = YRatioToChart \* Chart.ChartObject.Height;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

