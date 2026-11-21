---
title: "RenderingWatermark"
second_title: "Aspose.Cells for Java API Referansı"
description: "Renderleme için filigran."
type: docs
url: /tr/java/com.aspose.cells/renderingwatermark/
---

**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```

Renderleme için filigran.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | Metin filigranının örneğini oluşturur. |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | Görüntü filigranının örneğini oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Filigranın yazı tipini alır. |
| [getHAlignment()](#getHAlignment--) | Filigranın sayfaya göre yatay hizalamasını alır. |
| [getImage()](#getImage--) | Filigranın görüntüsünü alır. |
| [getOffsetX()](#getOffsetX--) | Ofset değerini alır [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [getOffsetY()](#getOffsetY--) | Ofset değerini alır [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [getOpacity()](#getOpacity--) | Filigranın opaklığını [0, 1] aralığında alır. |
| [getRotation()](#getRotation--) | Filigranın dönüş açısını derece cinsinden alır. |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | Hedef sayfaya göre ölçeği yüzde olarak alır. |
| [getText()](#getText--) | Filigranın metnini alır. |
| [getVAlignment()](#getVAlignment--) | Filigranın sayfaya göre dikey hizalamasını alır. |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | Filigranın sayfa içeriğinin arkasına yerleştirildiğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | Filigranın sayfa içeriğinin arkasına yerleştirildiğini gösterir. |
| [setHAlignment(int value)](#setHAlignment-int-) | Filigranın sayfaya göre yatay hizalamasını ayarlar. |
| [setOffsetX(float value)](#setOffsetX-float-) | Ofset değerini ayarlar [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | Ofset değerini ayarlar [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | Filigranın opaklığını [0, 1] aralığında ayarlar. |
| [setRotation(float value)](#setRotation-float-) | Filigranın dönüş açısını derece cinsinde ayarlar. |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | Hedef sayfaya göre ölçeği yüzde olarak ayarlar. |
| [setVAlignment(int value)](#setVAlignment-int-) | Filigranın sayfaya göre dikey hizalamasını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```


Metin filigranının örneğini oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | filigran metni |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | filigran yazı tipi |

### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```


Görüntü filigranının örneğini oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageData | byte[] |  |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public RenderingFont getFont()
```


Filigranın yazı tipini alır.

**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```


Filigranın sayfaya göre yatay hizalamasını alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Yalnızca Sol, Orta, Sağ geçerlidir. Varsayılan Sol'tur.

**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```


Filigranın görüntüsünü alır.

**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```


Ofset değerini alır [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```


Ofset değerini alır [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```


Filigranın opaklığını [0, 1] aralığında alır.

**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```


Filigranın dönüş açısını derece cinsinden alır.

**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```


Hedef sayfaya göre ölçeği yüzde olarak alır.

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Filigranın metnini alır.

**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```


Filigranın sayfaya göre dikey hizalamasını alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Yalnızca Üst, Orta, Alt geçerlidir. Varsayılan Üst'tür.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBackground() {#isBackground--}
```
public boolean isBackground()
```


Filigranın sayfa içeriğinin arkasına yerleştirildiğini gösterir.

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




### setBackground(boolean value) {#setBackground-boolean-}
```
public void setBackground(boolean value)
```


Filigranın sayfa içeriğinin arkasına yerleştirildiğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```


Filigranın sayfaya göre yatay hizalamasını ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Yalnızca Sol, Orta, Sağ geçerlidir. Varsayılan Sol'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```


Ofset değerini ayarlar [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```


Ofset değerini ayarlar [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```


Filigranın opaklığını [0, 1] aralığında ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```


Filigranın dönüş açısını derece cinsinde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```


Hedef sayfaya göre ölçeği yüzde olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```


Filigranın sayfaya göre dikey hizalamasını ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Yalnızca Üst, Orta, Alt geçerlidir. Varsayılan Üst'tür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

