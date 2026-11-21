---
title: "Title"
second_title: "Aspose.Cells for Java API Referansı"
description: "Grafik veya eksenin başlığını temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class Title extends ChartTextFrame
```

Grafik veya eksenin başlığını temsil eden nesneyi kapsüller.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [characters()](#characters--) | Bu Title öğesinin zengin metin biçimlendirmesini alır. |
| [characters(int startIndex, int length)](#characters-int-int-) | Metin içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Alır [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. |
| [getBackground()](#getBackground--) | Arka planın görüntüleme modunu alır. |
| [getBackgroundMode()](#getBackgroundMode--) | Arka planın görüntüleme modunu alır. |
| [getBorder()](#getBorder--) | Alır [Line](../../com.aspose.cells/line). |
| [getCharacters()](#getCharacters--) | Bu Title öğesinin zengin metin biçimlendirmesini alır. |
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
| [getFont()](#getFont--) | Belirtilen ChartFrame nesnesinin bir [getFont()](../../com.aspose.cells/chartframe\#getFont--) nesnesini alır. |
| [getHeight()](#getHeight--) | Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini alır. |
| [getHeightPixel()](#getHeightPixel--) | Çerçevenin yüksekliğini piksel biriminde alır. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Grafik alanının oran biriminde çerçevenin yüksekliğini alır. |
| [getLinkedSource()](#getLinkedSource--) | Çalışma sayfasına bir referans alır. |
| [getOverLay()](#getOverLay--) | Grafiği yeniden boyutlandırmadan, grafiğin ortasında bir kaplama başlığı temsil eder. |
| [getReadingOrder()](#getReadingOrder--) | Metin okuma sırasını temsil eder. |
| [getRotationAngle()](#getRotationAngle--) | Metin döndürme açısını temsil eder. |
| [getShadow()](#getShadow--) | Çerçevenin gölgesi varsa doğru. |
| [getShapeProperties()](#getShapeProperties--) | [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) nesnesini alır. |
| [getText()](#getText--) | Görüntü birimi etiketinin metnini alır. |
| [getTextDirection()](#getTextDirection--) | Metin okuma sırasını temsil eder. |
| [getTextFont()](#getTextFont--) | Belirtilen ChartFrame nesnesinin bir [getFont()](../../com.aspose.cells/chartframe\#getFont--) nesnesini alır. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Metnin yatay hizalamasını alır. |
| [getTextOptions()](#getTextOptions--) | Metnin seçeneklerini alır. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Metnin dikey hizalamasını alır. |
| [getWidth()](#getWidth--) | Grafik alanının 1/4000 biriminde çerçevenin genişliğini alır. |
| [getWidthPixel()](#getWidthPixel--) | Çerçevenin genişliğini piksel biriminde alır. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Grafik alanının oran biriminde çerçevenin genişliğini alır. |
| [getX()](#getX--) | Grafik alanının 1/4000 biriminde sol üst köşenin X koordinatını alır. |
| [getXPixel()](#getXPixel--) | Sol üst köşenin x koordinatını piksel biriminde alır. |
| [getXRatioToChart()](#getXRatioToChart--) | Grafik alanının Kesir biriminde sol üst köşenin x koordinatını alır. |
| [getY()](#getY--) | Grafik alanının 1/4000 biriminde sol üst köşenin y koordinatını alır. |
| [getYPixel()](#getYPixel--) | Piksel biriminde sol üst köşenin y koordinatını alır. |
| [getYRatioToChart()](#getYRatioToChart--) | Grafik alanının Kesir biriminde sol üst köşenin y koordinatını alır. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Grafiğin metninin otomatik olarak döndürülüp döndürülmediğini gösterir. |
| [isAutomaticSize()](#isAutomaticSize--) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir. |
| [isDeleted()](#isDeleted--) | Bu veri etiketinin silinip silinmediğini gösterir. |
| [isInnerMode()](#isInnerMode--) | Çizim alanı boyutunun işaretçileri ve eksen etiketlerini içerip içermediğini gösterir. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Bir şeklin içinde tanımlanan metni tamamen içerecek şekilde otomatik sığdırılıp sığdırılmayacağını alır. |
| [isTextWrapped()](#isTextWrapped--) | Metnin kaydırılıp kaydırılmadığını gösteren bir değeri alır. |
| [isVisible()](#isVisible--) | Başlığın görünür olup olmadığını temsil eder. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [setBackground(int value)](#setBackground-int-) | Arka planın görüntüleme modunu ayarlar. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Arka planın görüntüleme modunu ayarlar. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Bu veri etiketinin silinip silinmediğini gösterir. |
| [setDirectionType(int value)](#setDirectionType-int-) | Metnin yönünü ayarlar. |
| [setHeight(int value)](#setHeight-int-) | Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini ayarlar. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Piksel biriminde çerçevenin yüksekliğini ayarlar. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Grafik alanının oran biriminde çerçevenin yüksekliğini ayarlar. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Çizim alanı boyutunun işaretçileri ve eksen etiketlerini içerip içermediğini gösterir. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Çalışma sayfasına bir referans ayarlar. |
| [setOverLay(boolean value)](#setOverLay-boolean-) | Grafiği yeniden boyutlandırmadan, grafiğin ortasında bir kaplama başlığı temsil eder. |
| [setPositionAuto()](#setPositionAuto--) | Çerçevenin konumunu otomatik olarak ayarla |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Metin okuma sırasını temsil eder. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Bir şeklin içinde tanımlanan metni tamamen içerecek şekilde otomatik sığdırılıp sığdırılmayacağını ayarlar. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Metin döndürme açısını temsil eder. |
| [setShadow(boolean value)](#setShadow-boolean-) | Çerçevenin gölgesi varsa doğru. |
| [setText(String value)](#setText-java.lang.String-) | Görüntü birimi etiketinin metnini ayarlar. |
| [setTextDirection(int value)](#setTextDirection-int-) | Metin okuma sırasını temsil eder. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Metnin yatay hizalamasını ayarlar. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Metnin dikey hizalamasını ayarlar. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Metnin kaydırılıp kaydırılmadığını gösteren bir değeri ayarlar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Başlığın görünür olup olmadığını temsil eder. |
| [setWidth(int value)](#setWidth-int-) | Çerçevenin genişliğini, grafik alanının 1/4000'i biriminde ayarlar. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Çerçevenin genişliğini piksel biriminde ayarlar. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Çerçevenin genişliğini, grafik alanının oranı biriminde ayarlar. |
| [setX(int value)](#setX-int-) | Üst sol köşenin X koordinatını, grafik alanının 1/4000'i biriminde ayarlar. |
| [setXPixel(int value)](#setXPixel-int-) | Üst sol köşenin x koordinatını piksel biriminde ayarlar. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Üst sol köşenin x koordinatını, grafik alanının kesir biriminde ayarlar. |
| [setY(int value)](#setY-int-) | Üst sol köşenin y koordinatını, grafik alanının 1/4000'i biriminde ayarlar. |
| [setYPixel(int value)](#setYPixel-int-) | Üst sol köşenin y koordinatını piksel biriminde ayarlar. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Üst sol köşenin y koordinatını, grafik alanının kesir biriminde ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters() {#characters--}
```
public FontSetting[] characters()
```


Bu Title öğesinin zengin metin biçimlendirmesini alır.

**Returns:**
com.aspose.cells.FontSetting[] - FontSetting dizisini döndürür
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


Alır [getArea()](../../com.aspose.cells/chartframe\#getArea--).

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


Arka planın görüntüleme modunu alır. Bu özellik yalnızca Excel 2003 ve önceki sürümlerde geçerlidir.

Bakınız [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.Area.FillFormat.FillType** özelliğini kullanın. Örneğin, BackgroundMode'u Opaque olarak ayarlamanız gerekiyorsa, aşağıdaki kodu kullanabilirsiniz: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Bu özellik, ŞUBAT 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Alır [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Bu Title öğesinin zengin metin biçimlendirmesini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Title.Characters() metodunu kullanın. Bu özellik, KASIM 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
com.aspose.cells.FontSetting[] - FontSetting dizisini döndürür
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


Belirtilen ChartFrame nesnesinin bir [getFont()](../../com.aspose.cells/chartframe\#getFont--) nesnesini alır.

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
### getOverLay() {#getOverLay--}
```
public boolean getOverLay()
```


Grafiği yeniden boyutlandırmadan, grafiğin ortasında bir kaplama başlığı temsil eder.

**Returns:**
boolean
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
### getText() {#getText--}
```
public String getText()
```


Görüntü birimi etiketinin metnini alır.

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


Grafik alanının 1/4000 biriminde sol üst köşenin X koordinatını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Title.XRatioToChart özelliğini kullanın. X = XRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

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


Grafik alanının Kesir biriminde sol üst köşenin x koordinatını alır. Piksel cinsinden X = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Grafik alanının 1/4000 biriminde sol üst köşenin y koordinatını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Title.YRatioToChart özelliğini kullanın. Y = YRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

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


Grafik alanının Kesir biriminde sol üst köşenin y koordinatını alır. Piksel cinsinden Y = YRatioToChart \* Chart.ChartObject.Width;

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
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Başlığın görünür olup olmadığını temsil eder.

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


Arka planın görüntüleme modunu ayarlar. Bu özellik yalnızca Excel 2003 ve daha önceki sürümlerde geçerlidir.

Bakınız [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen **ChartFrame.Area.FillFormat.FillType** özelliğini kullanın. Örneğin, BackgroundMode'u Opaque olarak ayarlamanız gerekiyorsa, aşağıdaki kodu kullanabilirsiniz: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Bu özellik, ŞUBAT 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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

### setOverLay(boolean value) {#setOverLay-boolean-}
```
public void setOverLay(boolean value)
```


Grafiği yeniden boyutlandırmadan, grafiğin ortasında bir kaplama başlığı temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Görüntü birimi etiketinin metnini ayarlar.

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

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Başlığın görünür olup olmadığını temsil eder.

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


Üst sol köşenin X koordinatını, grafik alanının 1/4000'i biriminde ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Title.XRatioToChart özelliğini kullanın. X = XRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

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


Grafik alanının Kesir biriminde sol üst köşenin x koordinatını ayarlar. Piksel cinsinden X = XRatioToChart \* Chart.ChartObject.Width;

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

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Title.YRatioToChart özelliğini kullanın. Y = YRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

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


Grafik alanının Kesir biriminde sol üst köşenin y koordinatını ayarlar. Piksel cinsinden Y = YRatioToChart \* Chart.ChartObject.Width;

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

