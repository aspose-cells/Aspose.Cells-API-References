---
title: "CellsColor"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tüm renk türlerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/cellscolor/
---

**Inheritance:**
java.lang.Object
```
public class CellsColor
```

Tüm renk türlerini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | 32 bitlik ARGB değerinden rengi alır. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | RGB rengini alır. |
| [getColorIndex()](#getColorIndex--) | Renk paletindeki renk indeksini alır. |
| [getThemeColor()](#getThemeColor--) | Tema rengini alır. |
| [getTransparency()](#getTransparency--) | Şeffaflığı 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır. |
| [getType()](#getType--) | Renk türü. |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | Hücreye veya şekle uygulanması gereken rengi alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | 32 bitlik ARGB değerinden rengi ayarlar. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | RGB rengini ayarlar. |
| [setColorIndex(int value)](#setColorIndex-int-) | Renk paletindeki renk indeksini ayarlar. |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | Hücreye veya şekle uygulanması gereken rengi ayarlar. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Tema rengini alır. |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | Şekil renginin tonunu ayarla |
| [setTransparency(double value)](#setTransparency-double-) | Şeffaflığı 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak ayarlar. |
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
### getArgb() {#getArgb--}
```
public int getArgb()
```


32 bitlik ARGB değerinden rengi alır.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


RGB rengini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```


Renk paletindeki renk indeksini alır. Yalnızca indeksli renkler için geçerlidir.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Tema rengini alır. Yalnızca tema renk türü için geçerlidir.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Şeffaflığı 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır.

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Renk türü.

Bakın [ColorType](../../com.aspose.cells/colortype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isShapeColor() {#isShapeColor--}
```
public boolean isShapeColor()
```


Hücreye veya şekle uygulanması gereken rengi alır.

**Remarks**

Hücre ve şeklin renk ifadesi farklıdır. Örneğin, aynı ton değerine sahip tema rengi hücrede ve şekilde aynı olmayacaktır.

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




### setArgb(int value) {#setArgb-int-}
```
public void setArgb(int value)
```


32 bitlik ARGB değerinden rengi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


RGB rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```


Renk paletindeki renk indeksini ayarlar. Yalnızca indeksli renkler için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```


Hücreye veya şekle uygulanması gereken rengi ayarlar.

**Remarks**

Hücre ve şeklin renk ifadesi farklıdır. Örneğin, aynı ton değerine sahip tema rengi hücrede ve şekilde aynı olmayacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Tema rengini alır. Yalnızca tema renk türü için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```


Şekil renginin tonunu ayarla

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tint | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Şeffaflığı 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak ayarlar.

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

