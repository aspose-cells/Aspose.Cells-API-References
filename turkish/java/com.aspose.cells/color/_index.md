---
title: "Color"
second_title: "Aspose.Cells for Java API Referansı"
description: "ARGB alfa kırmızı yeşil mavi renk değerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/color/
---

**Inheritance:**
java.lang.Object
```
public class Color
```

ARGB (alfa, kırmızı, yeşil, mavi) rengini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Color()](#Color--) | yapıcı fonksiyon |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Belirtilen nesnenin bir Color nesnesi olup olmadığını ve bu nesneyle eşdeğer olup olmadığını test eder. |
| [fromArgb(int argb)](#fromArgb-int-) | 32 bitlik ARGB değerinden bir Color nesnesi oluşturur. |
| [fromArgb(int red, int green, int blue)](#fromArgb-int-int-int-) | Belirtilen 8 bitlik renk değerlerinden (kırmızı, yeşil ve mavi) bir Color nesnesi oluşturur. |
| [fromArgb(int alpha, int red, int green, int blue)](#fromArgb-int-int-int-int-) | Dört ARGB bileşeninin (alfa, kırmızı, yeşil ve mavi) değerlerinden bir Color nesnesi oluşturur. |
| [getA()](#getA--) | Bu Color nesnesinin alfa bileşen değerini alır. |
| [getAliceBlue()](#getAliceBlue--) | Sistem tanımlı bir rengi al. |
| [getAntiqueWhite()](#getAntiqueWhite--) | Sistem tanımlı bir rengi al. |
| [getAqua()](#getAqua--) | Sistem tanımlı bir rengi al. |
| [getAquamarine()](#getAquamarine--) | Sistem tanımlı bir rengi al. |
| [getAzure()](#getAzure--) | Sistem tanımlı bir rengi al. |
| [getB()](#getB--) | Bu Color nesnesinin mavi bileşen değerini alır. |
| [getBeige()](#getBeige--) | Sistem tanımlı bir rengi al. |
| [getBisque()](#getBisque--) | Sistem tanımlı bir rengi al. |
| [getBlack()](#getBlack--) | Sistem tanımlı bir rengi al. |
| [getBlanchedAlmond()](#getBlanchedAlmond--) | Sistem tanımlı bir rengi al. |
| [getBlue()](#getBlue--) | Sistem tanımlı bir rengi al. |
| [getBlueViolet()](#getBlueViolet--) | Sistem tanımlı bir rengi al. |
| [getBrown()](#getBrown--) | Sistem tanımlı bir rengi al. |
| [getBurlyWood()](#getBurlyWood--) | Sistem tanımlı bir rengi al. |
| [getCadetBlue()](#getCadetBlue--) | Sistem tanımlı bir rengi al. |
| [getChartreuse()](#getChartreuse--) | Sistem tanımlı bir rengi al. |
| [getChocolate()](#getChocolate--) | Sistem tanımlı bir rengi al. |
| [getClass()](#getClass--) |  |
| [getCoral()](#getCoral--) | Sistem tanımlı bir rengi al. |
| [getCornflowerBlue()](#getCornflowerBlue--) | Sistem tanımlı bir rengi al. |
| [getCornsilk()](#getCornsilk--) | Sistem tanımlı bir rengi al. |
| [getCrimson()](#getCrimson--) | Sistem tanımlı bir rengi al. |
| [getCyan()](#getCyan--) | Sistem tanımlı bir rengi al. |
| [getDarkBlue()](#getDarkBlue--) | Sistem tanımlı bir rengi al. |
| [getDarkCyan()](#getDarkCyan--) | Sistem tanımlı bir rengi al. |
| [getDarkGoldenrod()](#getDarkGoldenrod--) | Sistem tanımlı bir rengi al. |
| [getDarkGray()](#getDarkGray--) | Sistem tanımlı bir rengi al. |
| [getDarkGreen()](#getDarkGreen--) | Sistem tanımlı bir rengi al. |
| [getDarkKhaki()](#getDarkKhaki--) | Sistem tanımlı bir rengi al. |
| [getDarkMagenta()](#getDarkMagenta--) | Sistem tanımlı bir rengi al. |
| [getDarkOliveGreen()](#getDarkOliveGreen--) | Sistem tanımlı bir rengi al. |
| [getDarkOrange()](#getDarkOrange--) | Sistem tanımlı bir rengi al. |
| [getDarkOrchid()](#getDarkOrchid--) | Sistem tanımlı bir rengi al. |
| [getDarkRed()](#getDarkRed--) | Sistem tanımlı bir rengi al. |
| [getDarkSalmon()](#getDarkSalmon--) | Sistem tanımlı bir rengi al. |
| [getDarkSeaGreen()](#getDarkSeaGreen--) | Sistem tanımlı bir rengi al. |
| [getDarkSlateBlue()](#getDarkSlateBlue--) | Sistem tanımlı bir rengi al. |
| [getDarkSlateGray()](#getDarkSlateGray--) | Sistem tanımlı bir rengi al. |
| [getDarkTurquoise()](#getDarkTurquoise--) | Sistem tanımlı bir rengi al. |
| [getDarkViolet()](#getDarkViolet--) | Sistem tanımlı bir rengi al. |
| [getDeepPink()](#getDeepPink--) | Sistem tanımlı bir rengi al. |
| [getDeepSkyBlue()](#getDeepSkyBlue--) | Sistem tanımlı bir rengi al. |
| [getDimGray()](#getDimGray--) | Sistem tanımlı bir rengi al. |
| [getDodgerBlue()](#getDodgerBlue--) | Sistem tanımlı bir rengi al. |
| [getEmpty()](#getEmpty--) | Sistem tanımlı boş bir rengi al. |
| [getFirebrick()](#getFirebrick--) | Sistem tanımlı bir rengi al. |
| [getFloralWhite()](#getFloralWhite--) | Sistem tanımlı bir rengi al. |
| [getForestGreen()](#getForestGreen--) | Sistem tanımlı bir rengi al. |
| [getFuchsia()](#getFuchsia--) | Sistem tanımlı bir rengi al. |
| [getG()](#getG--) | Bu Color nesnesinin yeşil bileşen değerini alır. |
| [getGainsboro()](#getGainsboro--) | Sistem tanımlı bir rengi al. |
| [getGhostWhite()](#getGhostWhite--) | Sistem tanımlı bir rengi al. |
| [getGold()](#getGold--) | Sistem tanımlı bir rengi al. |
| [getGoldenrod()](#getGoldenrod--) | Sistem tanımlı bir rengi al. |
| [getGray()](#getGray--) | Sistem tanımlı bir rengi al. |
| [getGreen()](#getGreen--) | Sistem tanımlı bir rengi al. |
| [getGreenYellow()](#getGreenYellow--) | Sistem tanımlı bir rengi al. |
| [getHoneydew()](#getHoneydew--) | Sistem tanımlı bir rengi al. |
| [getHotPink()](#getHotPink--) | Sistem tanımlı bir rengi al. |
| [getIndianRed()](#getIndianRed--) | Sistem tanımlı bir rengi al. |
| [getIndigo()](#getIndigo--) | Sistem tanımlı bir rengi al. |
| [getIvory()](#getIvory--) | Sistem tanımlı bir rengi al. |
| [getKhaki()](#getKhaki--) | Sistem tanımlı bir rengi al. |
| [getLavender()](#getLavender--) | Sistem tanımlı bir rengi al. |
| [getLavenderBlush()](#getLavenderBlush--) | Sistem tanımlı bir rengi al. |
| [getLawnGreen()](#getLawnGreen--) | Sistem tanımlı bir rengi al. |
| [getLemonChiffon()](#getLemonChiffon--) | Sistem tanımlı bir rengi al. |
| [getLightBlue()](#getLightBlue--) | Sistem tanımlı bir rengi al. |
| [getLightCoral()](#getLightCoral--) | Sistem tanımlı bir rengi al. |
| [getLightCyan()](#getLightCyan--) | Sistem tanımlı bir rengi al. |
| [getLightGoldenrodYellow()](#getLightGoldenrodYellow--) | Sistem tanımlı bir rengi al. |
| [getLightGray()](#getLightGray--) | Sistem tanımlı bir rengi al. |
| [getLightGreen()](#getLightGreen--) | Sistem tanımlı bir rengi al. |
| [getLightPink()](#getLightPink--) | Sistem tanımlı bir rengi al. |
| [getLightSalmon()](#getLightSalmon--) | Sistem tanımlı bir rengi al. |
| [getLightSeaGreen()](#getLightSeaGreen--) | Sistem tanımlı bir rengi al. |
| [getLightSkyBlue()](#getLightSkyBlue--) | Sistem tanımlı bir rengi al. |
| [getLightSlateGray()](#getLightSlateGray--) | Sistem tanımlı bir rengi al. |
| [getLightSteelBlue()](#getLightSteelBlue--) | Sistem tanımlı bir rengi al. |
| [getLightYellow()](#getLightYellow--) | Sistem tanımlı bir rengi al. |
| [getLime()](#getLime--) | Sistem tanımlı bir rengi al. |
| [getLimeGreen()](#getLimeGreen--) | Sistem tanımlı bir rengi al. |
| [getLinen()](#getLinen--) | Sistem tanımlı bir rengi al. |
| [getMagenta()](#getMagenta--) | Sistem tanımlı bir rengi al. |
| [getMaroon()](#getMaroon--) | Sistem tanımlı bir rengi al. |
| [getMediumAquamarine()](#getMediumAquamarine--) | Sistem tanımlı bir rengi al. |
| [getMediumBlue()](#getMediumBlue--) | Sistem tanımlı bir rengi al. |
| [getMediumOrchid()](#getMediumOrchid--) | Sistem tanımlı bir rengi al. |
| [getMediumPurple()](#getMediumPurple--) | Sistem tanımlı bir rengi al. |
| [getMediumSeaGreen()](#getMediumSeaGreen--) | Sistem tanımlı bir rengi al. |
| [getMediumSlateBlue()](#getMediumSlateBlue--) | Sistem tanımlı bir rengi al. |
| [getMediumSpringGreen()](#getMediumSpringGreen--) | Sistem tanımlı bir rengi al. |
| [getMediumTurquoise()](#getMediumTurquoise--) | Sistem tanımlı bir rengi al. |
| [getMediumVioletRed()](#getMediumVioletRed--) | Sistem tanımlı bir rengi al. |
| [getMidnightBlue()](#getMidnightBlue--) | Sistem tanımlı bir rengi al. |
| [getMintCream()](#getMintCream--) | Sistem tanımlı bir rengi al. |
| [getMistyRose()](#getMistyRose--) | Sistem tanımlı bir rengi al. |
| [getMoccasin()](#getMoccasin--) | Sistem tanımlı bir rengi al. |
| [getNavajoWhite()](#getNavajoWhite--) | Sistem tanımlı bir rengi al. |
| [getNavy()](#getNavy--) | Sistem tanımlı bir rengi al. |
| [getOldLace()](#getOldLace--) | Sistem tanımlı bir rengi al. |
| [getOlive()](#getOlive--) | Sistem tanımlı bir rengi al. |
| [getOliveDrab()](#getOliveDrab--) | Sistem tanımlı bir rengi al. |
| [getOrange()](#getOrange--) | Sistem tanımlı bir rengi al. |
| [getOrangeRed()](#getOrangeRed--) | Sistem tanımlı bir rengi al. |
| [getOrchid()](#getOrchid--) | Sistem tanımlı bir rengi al. |
| [getPaleGoldenrod()](#getPaleGoldenrod--) | Sistem tanımlı bir rengi al. |
| [getPaleGreen()](#getPaleGreen--) | Sistem tanımlı bir rengi al. |
| [getPaleTurquoise()](#getPaleTurquoise--) | Sistem tanımlı bir rengi al. |
| [getPaleVioletRed()](#getPaleVioletRed--) | Sistem tanımlı bir rengi al. |
| [getPapayaWhip()](#getPapayaWhip--) | Sistem tanımlı bir rengi al. |
| [getPeachPuff()](#getPeachPuff--) | Sistem tanımlı bir rengi al. |
| [getPeru()](#getPeru--) | Sistem tanımlı bir rengi al. |
| [getPink()](#getPink--) | Sistem tanımlı bir rengi al. |
| [getPlum()](#getPlum--) | Sistem tanımlı bir rengi al. |
| [getPowderBlue()](#getPowderBlue--) | Sistem tanımlı bir rengi al. |
| [getPurple()](#getPurple--) | Sistem tanımlı bir rengi al. |
| [getR()](#getR--) | Bu Color nesnesinin kırmızı bileşen değerini alır. |
| [getRed()](#getRed--) | Sistem tanımlı bir rengi al. |
| [getRosyBrown()](#getRosyBrown--) | Sistem tanımlı bir rengi al. |
| [getRoyalBlue()](#getRoyalBlue--) | Sistem tanımlı bir rengi al. |
| [getSaddleBrown()](#getSaddleBrown--) | Sistem tanımlı bir rengi al. |
| [getSalmon()](#getSalmon--) | Sistem tanımlı bir rengi al. |
| [getSandyBrown()](#getSandyBrown--) | Sistem tanımlı bir rengi al. |
| [getSeaGreen()](#getSeaGreen--) | Sistem tanımlı bir rengi al. |
| [getSeaShell()](#getSeaShell--) | Sistem tanımlı bir rengi al. |
| [getSienna()](#getSienna--) | Sistem tanımlı bir rengi al. |
| [getSilver()](#getSilver--) | Sistem tanımlı bir rengi al. |
| [getSkyBlue()](#getSkyBlue--) | Sistem tanımlı bir rengi al. |
| [getSlateBlue()](#getSlateBlue--) | Sistem tanımlı bir rengi al. |
| [getSlateGray()](#getSlateGray--) | Sistem tanımlı bir rengi al. |
| [getSnow()](#getSnow--) | Sistem tanımlı bir rengi al. |
| [getSpringGreen()](#getSpringGreen--) | Sistem tanımlı bir rengi al. |
| [getSteelBlue()](#getSteelBlue--) | Sistem tanımlı bir rengi al. |
| [getTan()](#getTan--) | Sistem tanımlı bir rengi al. |
| [getTeal()](#getTeal--) | Sistem tanımlı bir rengi al. |
| [getThistle()](#getThistle--) | Sistem tanımlı bir rengi al. |
| [getTomato()](#getTomato--) | Sistem tanımlı bir rengi al. |
| [getTransparent()](#getTransparent--) | Sistem tanımlı bir rengi al. |
| [getTurquoise()](#getTurquoise--) | Sistem tanımlı bir rengi al. |
| [getViolet()](#getViolet--) | Sistem tanımlı bir rengi al. |
| [getWheat()](#getWheat--) | Sistem tanımlı bir rengi al. |
| [getWhite()](#getWhite--) | Sistem tanımlı bir rengi al. |
| [getWhiteSmoke()](#getWhiteSmoke--) | Sistem tanımlı bir rengi al. |
| [getYellow()](#getYellow--) | Sistem tanımlı bir rengi al. |
| [getYellowGreen()](#getYellowGreen--) | Sistem tanımlı bir rengi al. |
| [hashCode()](#hashCode--) | Bu Color nesnesi için bir karma kodu döndürür. |
| [isEmpty()](#isEmpty--) | Bu Color nesnesinin başlatılmamış olup olmadığını belirtir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toArgb()](#toArgb--) | Bu Color nesnesinin 32 bitlik ARGB değerini alır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Color() {#Color--}
```
public Color()
```


yapıcı fonksiyon

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Belirtilen nesnenin bir Color nesnesi olup olmadığını ve bu nesneyle eşdeğer olup olmadığını test eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Test edilecek nesne. |

**Returns:**
boolean - obj bir Color nesnesi ve bu Color nesnesiyle eşdeğer ise true; aksi takdirde false.
### fromArgb(int argb) {#fromArgb-int-}
```
public static Color fromArgb(int argb)
```


32 bitlik ARGB değerinden bir Color nesnesi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| argb | int | 32 bitlik ARGB değerini belirten bir değer. |

**Returns:**
[Color](../../com.aspose.cells/color) - The Color object that this method creates.
### fromArgb(int red, int green, int blue) {#fromArgb-int-int-int-}
```
public static Color fromArgb(int red, int green, int blue)
```


Belirtilen 8 bitlik renk değerlerinden (kırmızı, yeşil ve mavi) bir Color nesnesi oluşturur. Alfa değeri dolaylı olarak 255 (tamamen opak) olarak ayarlanır. Bu yöntem her renk bileşeni için 32 bitlik bir değer geçirmeye izin verse de, her bileşenin değeri 8 bit ile sınırlıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kırmızı | int | Yeni Color nesnesinin kırmızı bileşen değeri. Geçerli değerler 0 ile 255 arasındadır. |
| yeşil | int | Yeni Color nesnesinin yeşil bileşen değeri. Geçerli değerler 0 ile 255 arasındadır. |
| mavi | int | Yeni Color nesnesinin mavi bileşen değeri. Geçerli değerler 0 ile 255 arasındadır. |

**Returns:**
[Color](../../com.aspose.cells/color) - The Color object that this method creates.
### fromArgb(int alpha, int red, int green, int blue) {#fromArgb-int-int-int-int-}
```
public static Color fromArgb(int alpha, int red, int green, int blue)
```


Dört ARGB bileşeninin (alfa, kırmızı, yeşil ve mavi) değerlerinden bir Color nesnesi oluşturur. Bu yöntem her bileşen için 32 bitlik bir değer geçirmeye izin verse de, her bileşenin değeri 8 bit ile sınırlıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alfa | int | Alfa bileşeni. Geçerli değerler 0 ile 255 arasındadır. |
| kırmızı | int | Kırmızı bileşeni. Geçerli değerler 0 ile 255 arasındadır. |
| yeşil | int | Yeşil bileşeni. Geçerli değerler 0 ile 255 arasındadır. |
| mavi | int | Mavi bileşeni. Geçerli değerler 0 ile 255 arasındadır. |

**Returns:**
[Color](../../com.aspose.cells/color) - The Color object that this method creates.
### getA() {#getA--}
```
public byte getA()
```


Bu Color nesnesinin alfa bileşen değerini alır.

**Returns:**
byte - Bu Color nesnesinin alfa bileşen değeri.
### getAliceBlue() {#getAliceBlue--}
```
public static Color getAliceBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getAntiqueWhite() {#getAntiqueWhite--}
```
public static Color getAntiqueWhite()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getAqua() {#getAqua--}
```
public static Color getAqua()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getAquamarine() {#getAquamarine--}
```
public static Color getAquamarine()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getAzure() {#getAzure--}
```
public static Color getAzure()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getB() {#getB--}
```
public byte getB()
```


Bu Color nesnesinin mavi bileşen değerini alır.

**Returns:**
byte - Bu Color nesnesinin mavi bileşen değeri.
### getBeige() {#getBeige--}
```
public static Color getBeige()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBisque() {#getBisque--}
```
public static Color getBisque()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBlack() {#getBlack--}
```
public static Color getBlack()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBlanchedAlmond() {#getBlanchedAlmond--}
```
public static Color getBlanchedAlmond()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBlue() {#getBlue--}
```
public static Color getBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBlueViolet() {#getBlueViolet--}
```
public static Color getBlueViolet()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBrown() {#getBrown--}
```
public static Color getBrown()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBurlyWood() {#getBurlyWood--}
```
public static Color getBurlyWood()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCadetBlue() {#getCadetBlue--}
```
public static Color getCadetBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getChartreuse() {#getChartreuse--}
```
public static Color getChartreuse()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getChocolate() {#getChocolate--}
```
public static Color getChocolate()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCoral() {#getCoral--}
```
public static Color getCoral()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCornflowerBlue() {#getCornflowerBlue--}
```
public static Color getCornflowerBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCornsilk() {#getCornsilk--}
```
public static Color getCornsilk()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCrimson() {#getCrimson--}
```
public static Color getCrimson()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCyan() {#getCyan--}
```
public static Color getCyan()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkBlue() {#getDarkBlue--}
```
public static Color getDarkBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkCyan() {#getDarkCyan--}
```
public static Color getDarkCyan()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkGoldenrod() {#getDarkGoldenrod--}
```
public static Color getDarkGoldenrod()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkGray() {#getDarkGray--}
```
public static Color getDarkGray()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkGreen() {#getDarkGreen--}
```
public static Color getDarkGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkKhaki() {#getDarkKhaki--}
```
public static Color getDarkKhaki()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkMagenta() {#getDarkMagenta--}
```
public static Color getDarkMagenta()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkOliveGreen() {#getDarkOliveGreen--}
```
public static Color getDarkOliveGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkOrange() {#getDarkOrange--}
```
public static Color getDarkOrange()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkOrchid() {#getDarkOrchid--}
```
public static Color getDarkOrchid()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkRed() {#getDarkRed--}
```
public static Color getDarkRed()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkSalmon() {#getDarkSalmon--}
```
public static Color getDarkSalmon()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkSeaGreen() {#getDarkSeaGreen--}
```
public static Color getDarkSeaGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkSlateBlue() {#getDarkSlateBlue--}
```
public static Color getDarkSlateBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkSlateGray() {#getDarkSlateGray--}
```
public static Color getDarkSlateGray()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkTurquoise() {#getDarkTurquoise--}
```
public static Color getDarkTurquoise()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkViolet() {#getDarkViolet--}
```
public static Color getDarkViolet()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDeepPink() {#getDeepPink--}
```
public static Color getDeepPink()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDeepSkyBlue() {#getDeepSkyBlue--}
```
public static Color getDeepSkyBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDimGray() {#getDimGray--}
```
public static Color getDimGray()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDodgerBlue() {#getDodgerBlue--}
```
public static Color getDodgerBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getEmpty() {#getEmpty--}
```
public static Color getEmpty()
```


Sistem tanımlı boş bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getFirebrick() {#getFirebrick--}
```
public static Color getFirebrick()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getFloralWhite() {#getFloralWhite--}
```
public static Color getFloralWhite()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getForestGreen() {#getForestGreen--}
```
public static Color getForestGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getFuchsia() {#getFuchsia--}
```
public static Color getFuchsia()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getG() {#getG--}
```
public byte getG()
```


Bu Color nesnesinin yeşil bileşen değerini alır.

**Returns:**
byte - Bu Color nesnesinin yeşil bileşen değeri.
### getGainsboro() {#getGainsboro--}
```
public static Color getGainsboro()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGhostWhite() {#getGhostWhite--}
```
public static Color getGhostWhite()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGold() {#getGold--}
```
public static Color getGold()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGoldenrod() {#getGoldenrod--}
```
public static Color getGoldenrod()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGray() {#getGray--}
```
public static Color getGray()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGreen() {#getGreen--}
```
public static Color getGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGreenYellow() {#getGreenYellow--}
```
public static Color getGreenYellow()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getHoneydew() {#getHoneydew--}
```
public static Color getHoneydew()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getHotPink() {#getHotPink--}
```
public static Color getHotPink()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getIndianRed() {#getIndianRed--}
```
public static Color getIndianRed()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getIndigo() {#getIndigo--}
```
public static Color getIndigo()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getIvory() {#getIvory--}
```
public static Color getIvory()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getKhaki() {#getKhaki--}
```
public static Color getKhaki()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLavender() {#getLavender--}
```
public static Color getLavender()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLavenderBlush() {#getLavenderBlush--}
```
public static Color getLavenderBlush()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLawnGreen() {#getLawnGreen--}
```
public static Color getLawnGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLemonChiffon() {#getLemonChiffon--}
```
public static Color getLemonChiffon()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightBlue() {#getLightBlue--}
```
public static Color getLightBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightCoral() {#getLightCoral--}
```
public static Color getLightCoral()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightCyan() {#getLightCyan--}
```
public static Color getLightCyan()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightGoldenrodYellow() {#getLightGoldenrodYellow--}
```
public static Color getLightGoldenrodYellow()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightGray() {#getLightGray--}
```
public static Color getLightGray()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightGreen() {#getLightGreen--}
```
public static Color getLightGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightPink() {#getLightPink--}
```
public static Color getLightPink()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSalmon() {#getLightSalmon--}
```
public static Color getLightSalmon()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSeaGreen() {#getLightSeaGreen--}
```
public static Color getLightSeaGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSkyBlue() {#getLightSkyBlue--}
```
public static Color getLightSkyBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSlateGray() {#getLightSlateGray--}
```
public static Color getLightSlateGray()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSteelBlue() {#getLightSteelBlue--}
```
public static Color getLightSteelBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightYellow() {#getLightYellow--}
```
public static Color getLightYellow()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLime() {#getLime--}
```
public static Color getLime()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLimeGreen() {#getLimeGreen--}
```
public static Color getLimeGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLinen() {#getLinen--}
```
public static Color getLinen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMagenta() {#getMagenta--}
```
public static Color getMagenta()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMaroon() {#getMaroon--}
```
public static Color getMaroon()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumAquamarine() {#getMediumAquamarine--}
```
public static Color getMediumAquamarine()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumBlue() {#getMediumBlue--}
```
public static Color getMediumBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumOrchid() {#getMediumOrchid--}
```
public static Color getMediumOrchid()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumPurple() {#getMediumPurple--}
```
public static Color getMediumPurple()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumSeaGreen() {#getMediumSeaGreen--}
```
public static Color getMediumSeaGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumSlateBlue() {#getMediumSlateBlue--}
```
public static Color getMediumSlateBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumSpringGreen() {#getMediumSpringGreen--}
```
public static Color getMediumSpringGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumTurquoise() {#getMediumTurquoise--}
```
public static Color getMediumTurquoise()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumVioletRed() {#getMediumVioletRed--}
```
public static Color getMediumVioletRed()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMidnightBlue() {#getMidnightBlue--}
```
public static Color getMidnightBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMintCream() {#getMintCream--}
```
public static Color getMintCream()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMistyRose() {#getMistyRose--}
```
public static Color getMistyRose()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMoccasin() {#getMoccasin--}
```
public static Color getMoccasin()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getNavajoWhite() {#getNavajoWhite--}
```
public static Color getNavajoWhite()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getNavy() {#getNavy--}
```
public static Color getNavy()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOldLace() {#getOldLace--}
```
public static Color getOldLace()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOlive() {#getOlive--}
```
public static Color getOlive()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOliveDrab() {#getOliveDrab--}
```
public static Color getOliveDrab()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOrange() {#getOrange--}
```
public static Color getOrange()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOrangeRed() {#getOrangeRed--}
```
public static Color getOrangeRed()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOrchid() {#getOrchid--}
```
public static Color getOrchid()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPaleGoldenrod() {#getPaleGoldenrod--}
```
public static Color getPaleGoldenrod()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPaleGreen() {#getPaleGreen--}
```
public static Color getPaleGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPaleTurquoise() {#getPaleTurquoise--}
```
public static Color getPaleTurquoise()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPaleVioletRed() {#getPaleVioletRed--}
```
public static Color getPaleVioletRed()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPapayaWhip() {#getPapayaWhip--}
```
public static Color getPapayaWhip()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPeachPuff() {#getPeachPuff--}
```
public static Color getPeachPuff()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPeru() {#getPeru--}
```
public static Color getPeru()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPink() {#getPink--}
```
public static Color getPink()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPlum() {#getPlum--}
```
public static Color getPlum()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPowderBlue() {#getPowderBlue--}
```
public static Color getPowderBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPurple() {#getPurple--}
```
public static Color getPurple()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getR() {#getR--}
```
public byte getR()
```


Bu Color nesnesinin kırmızı bileşen değerini alır.

**Returns:**
byte - Bu Color nesnesinin kırmızı bileşen değeri.
### getRed() {#getRed--}
```
public static Color getRed()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getRosyBrown() {#getRosyBrown--}
```
public static Color getRosyBrown()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getRoyalBlue() {#getRoyalBlue--}
```
public static Color getRoyalBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSaddleBrown() {#getSaddleBrown--}
```
public static Color getSaddleBrown()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSalmon() {#getSalmon--}
```
public static Color getSalmon()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSandyBrown() {#getSandyBrown--}
```
public static Color getSandyBrown()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSeaGreen() {#getSeaGreen--}
```
public static Color getSeaGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSeaShell() {#getSeaShell--}
```
public static Color getSeaShell()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSienna() {#getSienna--}
```
public static Color getSienna()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSilver() {#getSilver--}
```
public static Color getSilver()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSkyBlue() {#getSkyBlue--}
```
public static Color getSkyBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSlateBlue() {#getSlateBlue--}
```
public static Color getSlateBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSlateGray() {#getSlateGray--}
```
public static Color getSlateGray()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSnow() {#getSnow--}
```
public static Color getSnow()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSpringGreen() {#getSpringGreen--}
```
public static Color getSpringGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSteelBlue() {#getSteelBlue--}
```
public static Color getSteelBlue()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTan() {#getTan--}
```
public static Color getTan()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTeal() {#getTeal--}
```
public static Color getTeal()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getThistle() {#getThistle--}
```
public static Color getThistle()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTomato() {#getTomato--}
```
public static Color getTomato()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTransparent() {#getTransparent--}
```
public static Color getTransparent()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTurquoise() {#getTurquoise--}
```
public static Color getTurquoise()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getViolet() {#getViolet--}
```
public static Color getViolet()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getWheat() {#getWheat--}
```
public static Color getWheat()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getWhite() {#getWhite--}
```
public static Color getWhite()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getWhiteSmoke() {#getWhiteSmoke--}
```
public static Color getWhiteSmoke()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getYellow() {#getYellow--}
```
public static Color getYellow()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getYellowGreen() {#getYellowGreen--}
```
public static Color getYellowGreen()
```


Sistem tanımlı bir rengi al.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Bu Color nesnesi için bir karma kodu döndürür.

**Returns:**
int - Bu Color nesnesi için hash kodunu belirten bir tam sayı değeri.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Bu Color nesnesinin başlatılmamış olup olmadığını belirtir.

**Returns:**
boolean - Bu özellik, renk başlatılmamışsa true döndürür; aksi takdirde false.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toArgb() {#toArgb--}
```
public int toArgb()
```


Bu Color nesnesinin 32 bitlik ARGB değerini alır.

**Returns:**
int - Bu Color nesnesinin 32-bit ARGB değeri.
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

