---
title: "ChartFrame"
second_title: "Aspose.Cells for Java API Referansı"
description: "Grafikteki çerçeve nesnesini temsil eden nesneyi kapsar."
type: docs
url: /tr/java/com.aspose.cells/chartframe/
---

**Inheritance:**
java.lang.Object
```
public class ChartFrame
```

Grafikteki çerçeve nesnesini temsil eden nesneyi kapsar.
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
| [getHeight()](#getHeight--) | Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini alır. |
| [getHeightPixel()](#getHeightPixel--) | Çerçevenin yüksekliğini piksel biriminde alır. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Grafik alanının oran biriminde çerçevenin yüksekliğini alır. |
| [getShadow()](#getShadow--) | Çerçevenin gölgesi varsa doğru. |
| [getShapeProperties()](#getShapeProperties--) | [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) nesnesini alır. |
| [getTextFont()](#getTextFont--) | Belirtilen ChartFrame nesnesinin bir [getFont()](../../com.aspose.cells/chartframe\#getFont--) nesnesini alır. |
| [getTextOptions()](#getTextOptions--) | Metnin seçeneklerini alır. |
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
| [isAutomaticSize()](#isAutomaticSize--) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir. |
| [isInnerMode()](#isInnerMode--) | Çizim alanı boyutunun işaretçileri ve eksen etiketlerini içerip içermediğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [setBackground(int value)](#setBackground-int-) | Arka planın görüntüleme modunu ayarlar. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Arka planın görüntüleme modunu ayarlar. |
| [setHeight(int value)](#setHeight-int-) | Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini ayarlar. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Piksel biriminde çerçevenin yüksekliğini ayarlar. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Grafik alanının oran biriminde çerçevenin yüksekliğini ayarlar. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Çizim alanı boyutunun işaretçileri ve eksen etiketlerini içerip içermediğini gösterir. |
| [setPositionAuto()](#setPositionAuto--) | Çerçevenin konumunu otomatik olarak ayarla |
| [setShadow(boolean value)](#setShadow-boolean-) | Çerçevenin gölgesi varsa doğru. |
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

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Çerçevenin konumunu otomatik olarak ayarla

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

