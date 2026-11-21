---
title: "PlotArea"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir grafikte çizim alanını temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/plotarea/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe)
```
public class PlotArea extends ChartFrame
```

Bir grafikte çizim alanını temsil eden nesneyi kapsüller.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Alır [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. |
| [getBackground()](#getBackground--) | Arka planın görüntüleme modunu alır. |
| [getBackgroundMode()](#getBackgroundMode--) | Arka planın görüntüleme modunu alır. |
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
| [getFont()](#getFont--) | Belirtilen ChartFrame nesnesinin bir [getFont()](../../com.aspose.cells/chartframe\#getFont--) nesnesini alır. |
| [getHeight()](#getHeight--) | Grafik alanının 1/4000 birimi cinsinden plot-area sınırlama kutusunun yüksekliğini alır. |
| [getHeightPixel()](#getHeightPixel--) | Çerçevenin yüksekliğini piksel biriminde alır. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Grafik alanının oran birimi cinsinden plot area sınırlama kutusunun yüksekliğini alır. |
| [getInnerHeight()](#getInnerHeight--) | Grafik alanının 1/4000 birimi cinsinden plot area yüksekliğini alır. |
| [getInnerHeightRatioToChart()](#getInnerHeightRatioToChart--) | Grafik alanının oran birimi cinsinden plot area yüksekliğini alır. |
| [getInnerWidth()](#getInnerWidth--) | Grafik alanının 1/4000 birimi cinsinden plot area genişliğini alır. |
| [getInnerWidthRatioToChart()](#getInnerWidthRatioToChart--) | Grafik alanının oran birimi cinsinden plot area genişliğini alır. |
| [getInnerX()](#getInnerX--) | Grafik alanının üst üst köşesinin x koordinatını grafik alanının 1/4000 birimi cinsinden alır. |
| [getInnerXRatioToChart()](#getInnerXRatioToChart--) | Grafik alanının üst üst köşesinin x koordinatını grafik alanının oran birimi cinsinden alır veya alır. |
| [getInnerY()](#getInnerY--) | Grafik alanının üst üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden alır. |
| [getInnerYRatioToChart()](#getInnerYRatioToChart--) | Grafik alanının üst üst köşesinin x koordinatını grafik alanının oran birimi cinsinden alır veya alır. |
| [getShadow()](#getShadow--) | Çerçevenin gölgesi varsa doğru. |
| [getShapeProperties()](#getShapeProperties--) | [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) nesnesini alır. |
| [getTextFont()](#getTextFont--) | Belirtilen ChartFrame nesnesinin bir [getFont()](../../com.aspose.cells/chartframe\#getFont--) nesnesini alır. |
| [getTextOptions()](#getTextOptions--) | Metnin seçeneklerini alır. |
| [getWidth()](#getWidth--) | Grafik alanı sınırlayıcı kutusunun genişliğini, grafik alanının 1/4000 birimi cinsinden alır. |
| [getWidthPixel()](#getWidthPixel--) | Çerçevenin genişliğini piksel biriminde alır. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Grafik alanı sınırlayıcı kutusunun genişliğini, grafik alanının oranı biriminde alır. |
| [getX()](#getX--) | Grafik alanı sınırlayıcı kutusunun sol üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden alır. |
| [getXPixel()](#getXPixel--) | Sol üst köşenin x koordinatını piksel biriminde alır. |
| [getXRatioToChart()](#getXRatioToChart--) | Grafik alanı sınırlayıcı kutusunun sol üst köşesinin x koordinatını, grafik alanının oranı olarak alır. |
| [getY()](#getY--) | Grafik alanı sınırlayıcı kutusunun üst üst köşesinin y koordinatını, grafik alanının 1/4000 birimi cinsinden alır. |
| [getYPixel()](#getYPixel--) | Piksel biriminde sol üst köşenin y koordinatını alır. |
| [getYRatioToChart()](#getYRatioToChart--) | Grafik alanı sınırlayıcı kutusunun üst üst köşesinin y koordinatını, grafik alanının oranı olarak alır. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticSize()](#isAutomaticSize--) | Grafik alanının otomatik olarak boyutlandırılıp boyutlandırılmadığını gösterir. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir. |
| [isInnerMode()](#isInnerMode--) | Çizim alanı boyutunun işaretçileri ve eksen etiketlerini içerip içermediğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Grafik alanının otomatik olarak boyutlandırılıp boyutlandırılmadığını gösterir. |
| [setBackground(int value)](#setBackground-int-) | Arka planın görüntüleme modunu ayarlar. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Arka planın görüntüleme modunu ayarlar. |
| [setHeight(int value)](#setHeight-int-) | Grafik alanı sınırlayıcı kutusunun yüksekliğini, grafik alanının 1/4000 birimi cinsinden ayarlar. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Piksel biriminde çerçevenin yüksekliğini ayarlar. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Grafik alanı sınırlayıcı kutusunun yüksekliğini, grafik alanının oranı biriminde ayarlar. |
| [setInnerHeight(int value)](#setInnerHeight-int-) | Grafik alanının yüksekliğini, grafik alanının 1/4000 birimi cinsinden ayarlar. |
| [setInnerHeightRatioToChart(double value)](#setInnerHeightRatioToChart-double-) | Grafik alanının yüksekliğini, grafik alanının oranı biriminde ayarlar. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Çizim alanı boyutunun işaretçileri ve eksen etiketlerini içerip içermediğini gösterir. |
| [setInnerWidth(int value)](#setInnerWidth-int-) | Grafik alanının genişliğini, grafik alanının 1/4000 birimi cinsinden ayarlar. |
| [setInnerWidthRatioToChart(double value)](#setInnerWidthRatioToChart-double-) | Grafik alanının genişliğini, grafik alanının oranı biriminde ayarlar. |
| [setInnerX(int value)](#setInnerX-int-) | Grafik alanının üst üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden ayarlar. |
| [setInnerXRatioToChart(double value)](#setInnerXRatioToChart-double-) | Grafik alanının üst üst köşesinin x koordinatını grafik alanının oran birimi cinsinden alır veya alır. |
| [setInnerY(int value)](#setInnerY-int-) | Grafik alanının üst üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden ayarlar. |
| [setInnerYRatioToChart(double value)](#setInnerYRatioToChart-double-) | Grafik alanının üst üst köşesinin x koordinatını grafik alanının oran birimi cinsinden alır veya alır. |
| [setPositionAuto()](#setPositionAuto--) | Grafik alanının konumunu otomatik olarak ayarlar. |
| [setShadow(boolean value)](#setShadow-boolean-) | Çerçevenin gölgesi varsa doğru. |
| [setWidth(int value)](#setWidth-int-) | Grafik alanı sınırlayıcı kutusunun genişliğini, grafik alanının 1/4000 birimi cinsinden ayarlar. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Çerçevenin genişliğini piksel biriminde ayarlar. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Grafik alanı sınırlayıcı kutusunun genişliğini, grafik alanının oranı biriminde ayarlar. |
| [setX(int value)](#setX-int-) | Grafik alanı sınırlayıcı kutusunun sol üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden ayarlar. |
| [setXPixel(int value)](#setXPixel-int-) | Üst sol köşenin x koordinatını piksel biriminde ayarlar. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Grafik alanı sınırlayıcı kutusunun sol üst köşesinin x koordinatını, grafik alanının oranı olarak ayarlar. |
| [setY(int value)](#setY-int-) | Grafik alanı sınırlayıcı kutusunun üst üst köşesinin y koordinatını, grafik alanının 1/4000 birimi cinsinden ayarlar. |
| [setYPixel(int value)](#setYPixel-int-) | Üst sol köşenin y koordinatını piksel biriminde ayarlar. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Grafik alanı sınırlayıcı kutusunun üst üst köşesinin y koordinatını, grafik alanının oranı olarak ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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


Grafik alanının 1/4000 birimi cinsinden plot-area sınırlama kutusunun yüksekliğini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.HeightRatioToChart özelliğini kullanın. Yükseklik = HeightRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

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


Grafik alanının oran birimi cinsinden plot area sınırlama kutusunun yüksekliğini alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

HeightPixel = HeightRatioToChart \* chart.ChartObject.Width. Not: HeightRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanacaktır.

**Returns:**
double
### getInnerHeight() {#getInnerHeight--}
```
public int getInnerHeight()
```


Grafik alanının 1/4000 birimi cinsinden plot area yüksekliğini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.InnerHeightRatioToChart özelliğini kullanın. InnerHeight = InnerHeightRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getInnerHeightRatioToChart() {#getInnerHeightRatioToChart--}
```
public double getInnerHeightRatioToChart()
```


Grafik alanının oran birimi cinsinden plot area yüksekliğini alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

InnerHeight in Pixel = InnerXRatioToChart \* chart.ChartObject.Width. Not: InnerHeightRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak True olarak ayarlanacaktır.

**Returns:**
double
### getInnerWidth() {#getInnerWidth--}
```
public int getInnerWidth()
```


Grafik alanının 1/4000 birimi cinsinden plot area genişliğini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.InnerWidthRatioToChart özelliğini kullanın. InnerWidth = InnerWidthRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getInnerWidthRatioToChart() {#getInnerWidthRatioToChart--}
```
public double getInnerWidthRatioToChart()
```


Grafik alanının oran birimi cinsinden plot area genişliğini alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

InnerWidth in Pixel = InnerXRatioToChart \* chart.ChartObject.Width. Not: InnerWidthRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak True olarak ayarlanacaktır.

**Returns:**
double
### getInnerX() {#getInnerX--}
```
public int getInnerX()
```


Grafik alanının üst üst köşesinin x koordinatını grafik alanının 1/4000 birimi cinsinden alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.InnerXRatioToChart özelliğini kullanın. InnerX = InnerXRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getInnerXRatioToChart() {#getInnerXRatioToChart--}
```
public double getInnerXRatioToChart()
```


Grafik alanının üst üst köşesinin x koordinatını grafik alanının oran birimi cinsinden alır veya alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

InnerX in Pixel = InnerXRatioToChart \* chart.ChartObject.Width. Not: InnerXRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak True olarak ayarlanacaktır.

**Returns:**
double
### getInnerY() {#getInnerY--}
```
public int getInnerY()
```


Grafik alanının üst üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.InnerYRatioToChart özelliğini kullanın. InnerY = InnerYRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getInnerYRatioToChart() {#getInnerYRatioToChart--}
```
public double getInnerYRatioToChart()
```


Grafik alanının üst üst köşesinin x koordinatını grafik alanının oran birimi cinsinden alır veya alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

InnerY in Pixel = InnerYRatioToChart \* chart.ChartObject.Width. Not: InnerYRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak True olarak ayarlanacaktır.

**Returns:**
double
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
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Belirtilen ChartFrame nesnesinin bir [getFont()](../../com.aspose.cells/chartframe\#getFont--) nesnesini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ChartFrame.Font özelliğini kullanın. Bu özellik, OCAK 2012'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Metnin seçeneklerini alır.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getWidth() {#getWidth--}
```
public int getWidth()
```


Grafik alanı sınırlayıcı kutusunun genişliğini, grafik alanının 1/4000 birimi cinsinden alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.WidthRatioToChart özelliğini kullanın. Width = WidthRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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


Grafik alanı sınırlayıcı kutusunun genişliğini, grafik alanının oranı biriminde alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

WidthPixel = WidthRatioToChart \* chart.ChartObject.Width. Not: WidthRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanacaktır.

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Grafik alanı sınırlayıcı kutusunun sol üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.XRatioToChart özelliğini kullanın. X = XRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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


Grafik alanı sınırlayıcı kutusunun sol üst köşesinin x koordinatını, grafik alanının oranı olarak alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

XPixel = XRatioToChart \* chart.ChartObject.Width. Not: XRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanacaktır.

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Grafik alanı sınırlayıcı kutusunun üst üst köşesinin y koordinatını, grafik alanının 1/4000 birimi cinsinden alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.YRatioToChart özelliğini kullanın. Y = YRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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


Grafik alanı sınırlayıcı kutusunun üst üst köşesinin y koordinatını, grafik alanının oranı olarak alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

YPixel = YRatioToChart \* chart.ChartObject.Width. Not: YRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanacaktır.

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


Grafik alanının otomatik olarak boyutlandırılıp boyutlandırılmadığını gösterir.

**Remarks**

NOT: IsAutomaticSize True olarak ayarlandığında, Width ve Height için manuel olarak belirlediğiniz değerler devre dışı bırakılacaktır.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir.

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

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Grafik alanının otomatik olarak boyutlandırılıp boyutlandırılmadığını gösterir.

**Remarks**

NOT: IsAutomaticSize True olarak ayarlandığında, Width ve Height için manuel olarak belirlediğiniz değerler devre dışı bırakılacaktır.

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

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Grafik alanı sınırlayıcı kutusunun yüksekliğini, grafik alanının 1/4000 birimi cinsinden ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.HeightRatioToChart özelliğini kullanın. Yükseklik = HeightRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

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


Grafik alanı sınırlayıcı kutusunun yüksekliğini, grafik alanının oranı biriminde ayarlar.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

HeightPixel = HeightRatioToChart \* chart.ChartObject.Width. Not: HeightRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setInnerHeight(int value) {#setInnerHeight-int-}
```
public void setInnerHeight(int value)
```


Grafik alanının yüksekliğini, grafik alanının 1/4000 birimi cinsinden ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.InnerHeightRatioToChart özelliğini kullanın. InnerHeight = InnerHeightRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setInnerHeightRatioToChart(double value) {#setInnerHeightRatioToChart-double-}
```
public void setInnerHeightRatioToChart(double value)
```


Grafik alanının yüksekliğini, grafik alanının oranı biriminde ayarlar.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

InnerHeight in Pixel = InnerXRatioToChart \* chart.ChartObject.Width. Not: InnerHeightRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak True olarak ayarlanacaktır.

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

### setInnerWidth(int value) {#setInnerWidth-int-}
```
public void setInnerWidth(int value)
```


Grafik alanının genişliğini, grafik alanının 1/4000 birimi cinsinden ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.InnerWidthRatioToChart özelliğini kullanın. InnerWidth = InnerWidthRatioToChart \* 4000; Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setInnerWidthRatioToChart(double value) {#setInnerWidthRatioToChart-double-}
```
public void setInnerWidthRatioToChart(double value)
```


Grafik alanının genişliğini, grafik alanının oranı biriminde ayarlar.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

InnerWidth in Pixel = InnerXRatioToChart \* chart.ChartObject.Width. Not: InnerWidthRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak True olarak ayarlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setInnerX(int value) {#setInnerX-int-}
```
public void setInnerX(int value)
```


Grafik alanının üst üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.InnerXRatioToChart özelliğini kullanın. InnerX = InnerXRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setInnerXRatioToChart(double value) {#setInnerXRatioToChart-double-}
```
public void setInnerXRatioToChart(double value)
```


Grafik alanının üst üst köşesinin x koordinatını grafik alanının oran birimi cinsinden alır veya alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

InnerX in Pixel = InnerXRatioToChart \* chart.ChartObject.Width. Not: InnerXRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak True olarak ayarlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setInnerY(int value) {#setInnerY-int-}
```
public void setInnerY(int value)
```


Grafik alanının üst üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.InnerYRatioToChart özelliğini kullanın. InnerY = InnerYRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setInnerYRatioToChart(double value) {#setInnerYRatioToChart-double-}
```
public void setInnerYRatioToChart(double value)
```


Grafik alanının üst üst köşesinin x koordinatını grafik alanının oran birimi cinsinden alır veya alır.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

InnerY in Pixel = InnerYRatioToChart \* chart.ChartObject.Width. Not: InnerYRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak True olarak ayarlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Grafik alanının konumunu otomatik olarak ayarlar.

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

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Grafik alanı sınırlayıcı kutusunun genişliğini, grafik alanının 1/4000 birimi cinsinden ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.WidthRatioToChart özelliğini kullanın. Width = WidthRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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


Grafik alanı sınırlayıcı kutusunun genişliğini, grafik alanının oranı biriminde ayarlar.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

WidthPixel = WidthRatioToChart \* chart.ChartObject.Width. Not: WidthRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Grafik alanı sınırlayıcı kutusunun sol üst köşesinin x koordinatını, grafik alanının 1/4000 birimi cinsinden ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.XRatioToChart özelliğini kullanın. X = XRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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


Grafik alanı sınırlayıcı kutusunun sol üst köşesinin x koordinatını, grafik alanının oranı olarak ayarlar.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

XPixel = XRatioToChart \* chart.ChartObject.Width. Not: XRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Grafik alanı sınırlayıcı kutusunun üst üst köşesinin y koordinatını, grafik alanının 1/4000 birimi cinsinden ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.YRatioToChart özelliğini kullanın. Y = YRatioToChart \* 4000. Bu özellik, Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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


Grafik alanı sınırlayıcı kutusunun üst üst köşesinin y koordinatını, grafik alanının oranı olarak ayarlar.

**Remarks**

Grafik alanı sınırlayıcı kutusu, grafik alanını, işaretçileri(tick labels) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() metodunu çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea** içinde, grafik alanı, işaretçileri (işaretçi etiketleri) ve işaretçilerin etrafındaki küçük bir kenarlık dahil olmak üzere grafik alanı sınırlama kutusunu temsil eder. Grafik alanının gerçek boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

YPixel = YRatioToChart \* chart.ChartObject.Width. Not: YRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanacaktır.

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

