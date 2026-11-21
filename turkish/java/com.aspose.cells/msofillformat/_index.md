---
title: "MsoFillFormat"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir şekil için doldurma biçimlendirmesini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/msofillformat/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormat
```

Bir şekil için doldurma biçimlendirmesini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Dosyanın arka plan rengini alır. |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | Dolgu ön rengini alır. |
| [getImageData()](#getImageData--) | Doku ve Resim dolgu verilerini alır. |
| [getTexture()](#getTexture--) | Doku dolgu tipini alır. |
| [getTransparency()](#getTransparency--) | Belirtilen dolgunun şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Dolgu olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | Dosyanın arka plan rengini ayarlar. |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | Dolgunun ön rengini ayarlar. |
| [setImageData(byte[] value)](#setImageData-byte---) | Doku ve Resim dolgu verilerini ayarlar. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Belirtilen dolguyu tek renkli bir degradeye ayarlar. |
| [setTransparency(double value)](#setTransparency-double-) | Belirtilen dolgunun şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Dolgu olup olmadığını gösterir. |
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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Dosyanın arka plan rengini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Dolgu ön rengini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Doku ve Resim dolgu verilerini alır.

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


Doku dolgu tipini alır.

Bakınız [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Belirtilen dolgunun şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Dolgu olup olmadığını gösterir.

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




### setBackColor(Color value) {#setBackColor-com.aspose.cells.Color-}
```
public void setBackColor(Color value)
```


Dosyanın arka plan rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


Dolgunun ön rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Doku ve Resim dolgu verilerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Belirtilen dolguyu tek renkli bir degradeye ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| derece | double | Degrade derecesi. 0.0 (karanlık) ile 1.0 (açık) arasında bir değer olabilir. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Belirtilen dolgunun şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Dolgu olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

