---
title: "Color"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en ARGB alfa röd grön blå-färg."
type: docs
url: /sv/java/com.aspose.cells/color/
---

**Inheritance:**
java.lang.Object
```
public class Color
```

Representerar en ARGB-färg (alpha, röd, grön, blå).
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [Color()](#Color--) | konstruktionsfunktion |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Testar om det angivna objektet är ett Color-objekt och är ekvivalent med detta objekt. |
| [fromArgb(int argb)](#fromArgb-int-) | Skapar ett Color-objekt från ett 32-bitars ARGB-värde. |
| [fromArgb(int red, int green, int blue)](#fromArgb-int-int-int-) | Skapar ett Color-objekt från de angivna 8-bitars färgvärdena (röd, grön och blå). |
| [fromArgb(int alpha, int red, int green, int blue)](#fromArgb-int-int-int-int-) | Skapar ett Color-objekt från de fyra ARGB-komponenterna (alpha, röd, grön och blå) värdena. |
| [getA()](#getA--) | Hämtar alfa-komponentens värde för detta Color-objekt. |
| [getAliceBlue()](#getAliceBlue--) | Hämta en systemdefinierad färg. |
| [getAntiqueWhite()](#getAntiqueWhite--) | Hämta en systemdefinierad färg. |
| [getAqua()](#getAqua--) | Hämta en systemdefinierad färg. |
| [getAquamarine()](#getAquamarine--) | Hämta en systemdefinierad färg. |
| [getAzure()](#getAzure--) | Hämta en systemdefinierad färg. |
| [getB()](#getB--) | Hämtar blå komponentens värde för detta Color-objekt. |
| [getBeige()](#getBeige--) | Hämta en systemdefinierad färg. |
| [getBisque()](#getBisque--) | Hämta en systemdefinierad färg. |
| [getBlack()](#getBlack--) | Hämta en systemdefinierad färg. |
| [getBlanchedAlmond()](#getBlanchedAlmond--) | Hämta en systemdefinierad färg. |
| [getBlue()](#getBlue--) | Hämta en systemdefinierad färg. |
| [getBlueViolet()](#getBlueViolet--) | Hämta en systemdefinierad färg. |
| [getBrown()](#getBrown--) | Hämta en systemdefinierad färg. |
| [getBurlyWood()](#getBurlyWood--) | Hämta en systemdefinierad färg. |
| [getCadetBlue()](#getCadetBlue--) | Hämta en systemdefinierad färg. |
| [getChartreuse()](#getChartreuse--) | Hämta en systemdefinierad färg. |
| [getChocolate()](#getChocolate--) | Hämta en systemdefinierad färg. |
| [getClass()](#getClass--) |  |
| [getCoral()](#getCoral--) | Hämta en systemdefinierad färg. |
| [getCornflowerBlue()](#getCornflowerBlue--) | Hämta en systemdefinierad färg. |
| [getCornsilk()](#getCornsilk--) | Hämta en systemdefinierad färg. |
| [getCrimson()](#getCrimson--) | Hämta en systemdefinierad färg. |
| [getCyan()](#getCyan--) | Hämta en systemdefinierad färg. |
| [getDarkBlue()](#getDarkBlue--) | Hämta en systemdefinierad färg. |
| [getDarkCyan()](#getDarkCyan--) | Hämta en systemdefinierad färg. |
| [getDarkGoldenrod()](#getDarkGoldenrod--) | Hämta en systemdefinierad färg. |
| [getDarkGray()](#getDarkGray--) | Hämta en systemdefinierad färg. |
| [getDarkGreen()](#getDarkGreen--) | Hämta en systemdefinierad färg. |
| [getDarkKhaki()](#getDarkKhaki--) | Hämta en systemdefinierad färg. |
| [getDarkMagenta()](#getDarkMagenta--) | Hämta en systemdefinierad färg. |
| [getDarkOliveGreen()](#getDarkOliveGreen--) | Hämta en systemdefinierad färg. |
| [getDarkOrange()](#getDarkOrange--) | Hämta en systemdefinierad färg. |
| [getDarkOrchid()](#getDarkOrchid--) | Hämta en systemdefinierad färg. |
| [getDarkRed()](#getDarkRed--) | Hämta en systemdefinierad färg. |
| [getDarkSalmon()](#getDarkSalmon--) | Hämta en systemdefinierad färg. |
| [getDarkSeaGreen()](#getDarkSeaGreen--) | Hämta en systemdefinierad färg. |
| [getDarkSlateBlue()](#getDarkSlateBlue--) | Hämta en systemdefinierad färg. |
| [getDarkSlateGray()](#getDarkSlateGray--) | Hämta en systemdefinierad färg. |
| [getDarkTurquoise()](#getDarkTurquoise--) | Hämta en systemdefinierad färg. |
| [getDarkViolet()](#getDarkViolet--) | Hämta en systemdefinierad färg. |
| [getDeepPink()](#getDeepPink--) | Hämta en systemdefinierad färg. |
| [getDeepSkyBlue()](#getDeepSkyBlue--) | Hämta en systemdefinierad färg. |
| [getDimGray()](#getDimGray--) | Hämta en systemdefinierad färg. |
| [getDodgerBlue()](#getDodgerBlue--) | Hämta en systemdefinierad färg. |
| [getEmpty()](#getEmpty--) | Hämta en systemdefinierad tom färg. |
| [getFirebrick()](#getFirebrick--) | Hämta en systemdefinierad färg. |
| [getFloralWhite()](#getFloralWhite--) | Hämta en systemdefinierad färg. |
| [getForestGreen()](#getForestGreen--) | Hämta en systemdefinierad färg. |
| [getFuchsia()](#getFuchsia--) | Hämta en systemdefinierad färg. |
| [getG()](#getG--) | Hämtar grön komponentens värde för detta Color-objekt. |
| [getGainsboro()](#getGainsboro--) | Hämta en systemdefinierad färg. |
| [getGhostWhite()](#getGhostWhite--) | Hämta en systemdefinierad färg. |
| [getGold()](#getGold--) | Hämta en systemdefinierad färg. |
| [getGoldenrod()](#getGoldenrod--) | Hämta en systemdefinierad färg. |
| [getGray()](#getGray--) | Hämta en systemdefinierad färg. |
| [getGreen()](#getGreen--) | Hämta en systemdefinierad färg. |
| [getGreenYellow()](#getGreenYellow--) | Hämta en systemdefinierad färg. |
| [getHoneydew()](#getHoneydew--) | Hämta en systemdefinierad färg. |
| [getHotPink()](#getHotPink--) | Hämta en systemdefinierad färg. |
| [getIndianRed()](#getIndianRed--) | Hämta en systemdefinierad färg. |
| [getIndigo()](#getIndigo--) | Hämta en systemdefinierad färg. |
| [getIvory()](#getIvory--) | Hämta en systemdefinierad färg. |
| [getKhaki()](#getKhaki--) | Hämta en systemdefinierad färg. |
| [getLavender()](#getLavender--) | Hämta en systemdefinierad färg. |
| [getLavenderBlush()](#getLavenderBlush--) | Hämta en systemdefinierad färg. |
| [getLawnGreen()](#getLawnGreen--) | Hämta en systemdefinierad färg. |
| [getLemonChiffon()](#getLemonChiffon--) | Hämta en systemdefinierad färg. |
| [getLightBlue()](#getLightBlue--) | Hämta en systemdefinierad färg. |
| [getLightCoral()](#getLightCoral--) | Hämta en systemdefinierad färg. |
| [getLightCyan()](#getLightCyan--) | Hämta en systemdefinierad färg. |
| [getLightGoldenrodYellow()](#getLightGoldenrodYellow--) | Hämta en systemdefinierad färg. |
| [getLightGray()](#getLightGray--) | Hämta en systemdefinierad färg. |
| [getLightGreen()](#getLightGreen--) | Hämta en systemdefinierad färg. |
| [getLightPink()](#getLightPink--) | Hämta en systemdefinierad färg. |
| [getLightSalmon()](#getLightSalmon--) | Hämta en systemdefinierad färg. |
| [getLightSeaGreen()](#getLightSeaGreen--) | Hämta en systemdefinierad färg. |
| [getLightSkyBlue()](#getLightSkyBlue--) | Hämta en systemdefinierad färg. |
| [getLightSlateGray()](#getLightSlateGray--) | Hämta en systemdefinierad färg. |
| [getLightSteelBlue()](#getLightSteelBlue--) | Hämta en systemdefinierad färg. |
| [getLightYellow()](#getLightYellow--) | Hämta en systemdefinierad färg. |
| [getLime()](#getLime--) | Hämta en systemdefinierad färg. |
| [getLimeGreen()](#getLimeGreen--) | Hämta en systemdefinierad färg. |
| [getLinen()](#getLinen--) | Hämta en systemdefinierad färg. |
| [getMagenta()](#getMagenta--) | Hämta en systemdefinierad färg. |
| [getMaroon()](#getMaroon--) | Hämta en systemdefinierad färg. |
| [getMediumAquamarine()](#getMediumAquamarine--) | Hämta en systemdefinierad färg. |
| [getMediumBlue()](#getMediumBlue--) | Hämta en systemdefinierad färg. |
| [getMediumOrchid()](#getMediumOrchid--) | Hämta en systemdefinierad färg. |
| [getMediumPurple()](#getMediumPurple--) | Hämta en systemdefinierad färg. |
| [getMediumSeaGreen()](#getMediumSeaGreen--) | Hämta en systemdefinierad färg. |
| [getMediumSlateBlue()](#getMediumSlateBlue--) | Hämta en systemdefinierad färg. |
| [getMediumSpringGreen()](#getMediumSpringGreen--) | Hämta en systemdefinierad färg. |
| [getMediumTurquoise()](#getMediumTurquoise--) | Hämta en systemdefinierad färg. |
| [getMediumVioletRed()](#getMediumVioletRed--) | Hämta en systemdefinierad färg. |
| [getMidnightBlue()](#getMidnightBlue--) | Hämta en systemdefinierad färg. |
| [getMintCream()](#getMintCream--) | Hämta en systemdefinierad färg. |
| [getMistyRose()](#getMistyRose--) | Hämta en systemdefinierad färg. |
| [getMoccasin()](#getMoccasin--) | Hämta en systemdefinierad färg. |
| [getNavajoWhite()](#getNavajoWhite--) | Hämta en systemdefinierad färg. |
| [getNavy()](#getNavy--) | Hämta en systemdefinierad färg. |
| [getOldLace()](#getOldLace--) | Hämta en systemdefinierad färg. |
| [getOlive()](#getOlive--) | Hämta en systemdefinierad färg. |
| [getOliveDrab()](#getOliveDrab--) | Hämta en systemdefinierad färg. |
| [getOrange()](#getOrange--) | Hämta en systemdefinierad färg. |
| [getOrangeRed()](#getOrangeRed--) | Hämta en systemdefinierad färg. |
| [getOrchid()](#getOrchid--) | Hämta en systemdefinierad färg. |
| [getPaleGoldenrod()](#getPaleGoldenrod--) | Hämta en systemdefinierad färg. |
| [getPaleGreen()](#getPaleGreen--) | Hämta en systemdefinierad färg. |
| [getPaleTurquoise()](#getPaleTurquoise--) | Hämta en systemdefinierad färg. |
| [getPaleVioletRed()](#getPaleVioletRed--) | Hämta en systemdefinierad färg. |
| [getPapayaWhip()](#getPapayaWhip--) | Hämta en systemdefinierad färg. |
| [getPeachPuff()](#getPeachPuff--) | Hämta en systemdefinierad färg. |
| [getPeru()](#getPeru--) | Hämta en systemdefinierad färg. |
| [getPink()](#getPink--) | Hämta en systemdefinierad färg. |
| [getPlum()](#getPlum--) | Hämta en systemdefinierad färg. |
| [getPowderBlue()](#getPowderBlue--) | Hämta en systemdefinierad färg. |
| [getPurple()](#getPurple--) | Hämta en systemdefinierad färg. |
| [getR()](#getR--) | Hämtar röd komponentens värde för detta Color-objekt. |
| [getRed()](#getRed--) | Hämta en systemdefinierad färg. |
| [getRosyBrown()](#getRosyBrown--) | Hämta en systemdefinierad färg. |
| [getRoyalBlue()](#getRoyalBlue--) | Hämta en systemdefinierad färg. |
| [getSaddleBrown()](#getSaddleBrown--) | Hämta en systemdefinierad färg. |
| [getSalmon()](#getSalmon--) | Hämta en systemdefinierad färg. |
| [getSandyBrown()](#getSandyBrown--) | Hämta en systemdefinierad färg. |
| [getSeaGreen()](#getSeaGreen--) | Hämta en systemdefinierad färg. |
| [getSeaShell()](#getSeaShell--) | Hämta en systemdefinierad färg. |
| [getSienna()](#getSienna--) | Hämta en systemdefinierad färg. |
| [getSilver()](#getSilver--) | Hämta en systemdefinierad färg. |
| [getSkyBlue()](#getSkyBlue--) | Hämta en systemdefinierad färg. |
| [getSlateBlue()](#getSlateBlue--) | Hämta en systemdefinierad färg. |
| [getSlateGray()](#getSlateGray--) | Hämta en systemdefinierad färg. |
| [getSnow()](#getSnow--) | Hämta en systemdefinierad färg. |
| [getSpringGreen()](#getSpringGreen--) | Hämta en systemdefinierad färg. |
| [getSteelBlue()](#getSteelBlue--) | Hämta en systemdefinierad färg. |
| [getTan()](#getTan--) | Hämta en systemdefinierad färg. |
| [getTeal()](#getTeal--) | Hämta en systemdefinierad färg. |
| [getThistle()](#getThistle--) | Hämta en systemdefinierad färg. |
| [getTomato()](#getTomato--) | Hämta en systemdefinierad färg. |
| [getTransparent()](#getTransparent--) | Hämta en systemdefinierad färg. |
| [getTurquoise()](#getTurquoise--) | Hämta en systemdefinierad färg. |
| [getViolet()](#getViolet--) | Hämta en systemdefinierad färg. |
| [getWheat()](#getWheat--) | Hämta en systemdefinierad färg. |
| [getWhite()](#getWhite--) | Hämta en systemdefinierad färg. |
| [getWhiteSmoke()](#getWhiteSmoke--) | Hämta en systemdefinierad färg. |
| [getYellow()](#getYellow--) | Hämta en systemdefinierad färg. |
| [getYellowGreen()](#getYellowGreen--) | Hämta en systemdefinierad färg. |
| [hashCode()](#hashCode--) | Returnerar en hashkod för detta Color-objekt. |
| [isEmpty()](#isEmpty--) | Anger om detta Color-objekt är oinitierat. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toArgb()](#toArgb--) | Hämtar 32-bitars ARGB-värdet för detta Color-objekt. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Color() {#Color--}
```
public Color()
```


konstruktionsfunktion

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Testar om det angivna objektet är ett Color-objekt och är ekvivalent med detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Objektet att testa. |

**Returns:**
boolean - true om obj är ett Color-objekt och motsvarar detta Color-objekt; annars false.
### fromArgb(int argb) {#fromArgb-int-}
```
public static Color fromArgb(int argb)
```


Skapar ett Color-objekt från ett 32-bitars ARGB-värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| argb | int | Ett värde som specificerar 32-bitars ARGB-värdet. |

**Returns:**
[Color](../../com.aspose.cells/color) - The Color object that this method creates.
### fromArgb(int red, int green, int blue) {#fromArgb-int-int-int-}
```
public static Color fromArgb(int red, int green, int blue)
```


Skapar ett Color-objekt från de angivna 8-bitars färgvärdena (röd, grön och blå). Alfa‑värdet är implicit 255 (fullt ogenomskinligt). Även om den här metoden tillåter att ett 32-bitars värde skickas för varje färgkomponent, är värdet för varje komponent begränsat till 8 bitar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| röd | int | Röd komponentvärde för det nya Color-objektet. Giltiga värden är 0 till 255. |
| grön | int | Grön komponentvärde för det nya Color-objektet. Giltiga värden är 0 till 255. |
| blå | int | Blå komponentvärde för det nya Color-objektet. Giltiga värden är 0 till 255. |

**Returns:**
[Color](../../com.aspose.cells/color) - The Color object that this method creates.
### fromArgb(int alpha, int red, int green, int blue) {#fromArgb-int-int-int-int-}
```
public static Color fromArgb(int alpha, int red, int green, int blue)
```


Skapar ett Color-objekt från de fyra ARGB-komponenterna (alpha, röd, grön och blå) värdena. Även om den här metoden tillåter att ett 32-bitars värde skickas för varje komponent, är värdet för varje komponent begränsat till 8 bitar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alpha | int | Alfa‑komponenten. Giltiga värden är 0 till 255. |
| röd | int | Röd komponent. Giltiga värden är 0 till 255. |
| grön | int | Grön komponent. Giltiga värden är 0 till 255. |
| blå | int | Den blå komponenten. Giltiga värden är 0 till 255. |

**Returns:**
[Color](../../com.aspose.cells/color) - The Color object that this method creates.
### getA() {#getA--}
```
public byte getA()
```


Hämtar alfa-komponentens värde för detta Color-objekt.

**Returns:**
byte - Alfa-komponentvärdet för detta Color-objekt.
### getAliceBlue() {#getAliceBlue--}
```
public static Color getAliceBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getAntiqueWhite() {#getAntiqueWhite--}
```
public static Color getAntiqueWhite()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getAqua() {#getAqua--}
```
public static Color getAqua()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getAquamarine() {#getAquamarine--}
```
public static Color getAquamarine()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getAzure() {#getAzure--}
```
public static Color getAzure()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getB() {#getB--}
```
public byte getB()
```


Hämtar blå komponentens värde för detta Color-objekt.

**Returns:**
byte - Det blå komponentvärdet för detta Color-objekt.
### getBeige() {#getBeige--}
```
public static Color getBeige()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBisque() {#getBisque--}
```
public static Color getBisque()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBlack() {#getBlack--}
```
public static Color getBlack()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBlanchedAlmond() {#getBlanchedAlmond--}
```
public static Color getBlanchedAlmond()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBlue() {#getBlue--}
```
public static Color getBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBlueViolet() {#getBlueViolet--}
```
public static Color getBlueViolet()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBrown() {#getBrown--}
```
public static Color getBrown()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getBurlyWood() {#getBurlyWood--}
```
public static Color getBurlyWood()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCadetBlue() {#getCadetBlue--}
```
public static Color getCadetBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getChartreuse() {#getChartreuse--}
```
public static Color getChartreuse()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getChocolate() {#getChocolate--}
```
public static Color getChocolate()
```


Hämta en systemdefinierad färg.

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


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCornflowerBlue() {#getCornflowerBlue--}
```
public static Color getCornflowerBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCornsilk() {#getCornsilk--}
```
public static Color getCornsilk()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCrimson() {#getCrimson--}
```
public static Color getCrimson()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getCyan() {#getCyan--}
```
public static Color getCyan()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkBlue() {#getDarkBlue--}
```
public static Color getDarkBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkCyan() {#getDarkCyan--}
```
public static Color getDarkCyan()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkGoldenrod() {#getDarkGoldenrod--}
```
public static Color getDarkGoldenrod()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkGray() {#getDarkGray--}
```
public static Color getDarkGray()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkGreen() {#getDarkGreen--}
```
public static Color getDarkGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkKhaki() {#getDarkKhaki--}
```
public static Color getDarkKhaki()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkMagenta() {#getDarkMagenta--}
```
public static Color getDarkMagenta()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkOliveGreen() {#getDarkOliveGreen--}
```
public static Color getDarkOliveGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkOrange() {#getDarkOrange--}
```
public static Color getDarkOrange()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkOrchid() {#getDarkOrchid--}
```
public static Color getDarkOrchid()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkRed() {#getDarkRed--}
```
public static Color getDarkRed()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkSalmon() {#getDarkSalmon--}
```
public static Color getDarkSalmon()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkSeaGreen() {#getDarkSeaGreen--}
```
public static Color getDarkSeaGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkSlateBlue() {#getDarkSlateBlue--}
```
public static Color getDarkSlateBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkSlateGray() {#getDarkSlateGray--}
```
public static Color getDarkSlateGray()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkTurquoise() {#getDarkTurquoise--}
```
public static Color getDarkTurquoise()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDarkViolet() {#getDarkViolet--}
```
public static Color getDarkViolet()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDeepPink() {#getDeepPink--}
```
public static Color getDeepPink()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDeepSkyBlue() {#getDeepSkyBlue--}
```
public static Color getDeepSkyBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDimGray() {#getDimGray--}
```
public static Color getDimGray()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getDodgerBlue() {#getDodgerBlue--}
```
public static Color getDodgerBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getEmpty() {#getEmpty--}
```
public static Color getEmpty()
```


Hämta en systemdefinierad tom färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getFirebrick() {#getFirebrick--}
```
public static Color getFirebrick()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getFloralWhite() {#getFloralWhite--}
```
public static Color getFloralWhite()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getForestGreen() {#getForestGreen--}
```
public static Color getForestGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getFuchsia() {#getFuchsia--}
```
public static Color getFuchsia()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getG() {#getG--}
```
public byte getG()
```


Hämtar grön komponentens värde för detta Color-objekt.

**Returns:**
byte - Det gröna komponentvärdet för detta Color-objekt.
### getGainsboro() {#getGainsboro--}
```
public static Color getGainsboro()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGhostWhite() {#getGhostWhite--}
```
public static Color getGhostWhite()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGold() {#getGold--}
```
public static Color getGold()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGoldenrod() {#getGoldenrod--}
```
public static Color getGoldenrod()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGray() {#getGray--}
```
public static Color getGray()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGreen() {#getGreen--}
```
public static Color getGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getGreenYellow() {#getGreenYellow--}
```
public static Color getGreenYellow()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getHoneydew() {#getHoneydew--}
```
public static Color getHoneydew()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getHotPink() {#getHotPink--}
```
public static Color getHotPink()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getIndianRed() {#getIndianRed--}
```
public static Color getIndianRed()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getIndigo() {#getIndigo--}
```
public static Color getIndigo()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getIvory() {#getIvory--}
```
public static Color getIvory()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getKhaki() {#getKhaki--}
```
public static Color getKhaki()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLavender() {#getLavender--}
```
public static Color getLavender()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLavenderBlush() {#getLavenderBlush--}
```
public static Color getLavenderBlush()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLawnGreen() {#getLawnGreen--}
```
public static Color getLawnGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLemonChiffon() {#getLemonChiffon--}
```
public static Color getLemonChiffon()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightBlue() {#getLightBlue--}
```
public static Color getLightBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightCoral() {#getLightCoral--}
```
public static Color getLightCoral()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightCyan() {#getLightCyan--}
```
public static Color getLightCyan()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightGoldenrodYellow() {#getLightGoldenrodYellow--}
```
public static Color getLightGoldenrodYellow()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightGray() {#getLightGray--}
```
public static Color getLightGray()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightGreen() {#getLightGreen--}
```
public static Color getLightGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightPink() {#getLightPink--}
```
public static Color getLightPink()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSalmon() {#getLightSalmon--}
```
public static Color getLightSalmon()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSeaGreen() {#getLightSeaGreen--}
```
public static Color getLightSeaGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSkyBlue() {#getLightSkyBlue--}
```
public static Color getLightSkyBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSlateGray() {#getLightSlateGray--}
```
public static Color getLightSlateGray()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightSteelBlue() {#getLightSteelBlue--}
```
public static Color getLightSteelBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLightYellow() {#getLightYellow--}
```
public static Color getLightYellow()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLime() {#getLime--}
```
public static Color getLime()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLimeGreen() {#getLimeGreen--}
```
public static Color getLimeGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getLinen() {#getLinen--}
```
public static Color getLinen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMagenta() {#getMagenta--}
```
public static Color getMagenta()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMaroon() {#getMaroon--}
```
public static Color getMaroon()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumAquamarine() {#getMediumAquamarine--}
```
public static Color getMediumAquamarine()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumBlue() {#getMediumBlue--}
```
public static Color getMediumBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumOrchid() {#getMediumOrchid--}
```
public static Color getMediumOrchid()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumPurple() {#getMediumPurple--}
```
public static Color getMediumPurple()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumSeaGreen() {#getMediumSeaGreen--}
```
public static Color getMediumSeaGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumSlateBlue() {#getMediumSlateBlue--}
```
public static Color getMediumSlateBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumSpringGreen() {#getMediumSpringGreen--}
```
public static Color getMediumSpringGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumTurquoise() {#getMediumTurquoise--}
```
public static Color getMediumTurquoise()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMediumVioletRed() {#getMediumVioletRed--}
```
public static Color getMediumVioletRed()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMidnightBlue() {#getMidnightBlue--}
```
public static Color getMidnightBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMintCream() {#getMintCream--}
```
public static Color getMintCream()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMistyRose() {#getMistyRose--}
```
public static Color getMistyRose()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getMoccasin() {#getMoccasin--}
```
public static Color getMoccasin()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getNavajoWhite() {#getNavajoWhite--}
```
public static Color getNavajoWhite()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getNavy() {#getNavy--}
```
public static Color getNavy()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOldLace() {#getOldLace--}
```
public static Color getOldLace()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOlive() {#getOlive--}
```
public static Color getOlive()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOliveDrab() {#getOliveDrab--}
```
public static Color getOliveDrab()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOrange() {#getOrange--}
```
public static Color getOrange()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOrangeRed() {#getOrangeRed--}
```
public static Color getOrangeRed()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getOrchid() {#getOrchid--}
```
public static Color getOrchid()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPaleGoldenrod() {#getPaleGoldenrod--}
```
public static Color getPaleGoldenrod()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPaleGreen() {#getPaleGreen--}
```
public static Color getPaleGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPaleTurquoise() {#getPaleTurquoise--}
```
public static Color getPaleTurquoise()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPaleVioletRed() {#getPaleVioletRed--}
```
public static Color getPaleVioletRed()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPapayaWhip() {#getPapayaWhip--}
```
public static Color getPapayaWhip()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPeachPuff() {#getPeachPuff--}
```
public static Color getPeachPuff()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPeru() {#getPeru--}
```
public static Color getPeru()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPink() {#getPink--}
```
public static Color getPink()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPlum() {#getPlum--}
```
public static Color getPlum()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPowderBlue() {#getPowderBlue--}
```
public static Color getPowderBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getPurple() {#getPurple--}
```
public static Color getPurple()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getR() {#getR--}
```
public byte getR()
```


Hämtar röd komponentens värde för detta Color-objekt.

**Returns:**
byte - Det röda komponentvärdet för detta Color-objekt.
### getRed() {#getRed--}
```
public static Color getRed()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getRosyBrown() {#getRosyBrown--}
```
public static Color getRosyBrown()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getRoyalBlue() {#getRoyalBlue--}
```
public static Color getRoyalBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSaddleBrown() {#getSaddleBrown--}
```
public static Color getSaddleBrown()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSalmon() {#getSalmon--}
```
public static Color getSalmon()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSandyBrown() {#getSandyBrown--}
```
public static Color getSandyBrown()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSeaGreen() {#getSeaGreen--}
```
public static Color getSeaGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSeaShell() {#getSeaShell--}
```
public static Color getSeaShell()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSienna() {#getSienna--}
```
public static Color getSienna()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSilver() {#getSilver--}
```
public static Color getSilver()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSkyBlue() {#getSkyBlue--}
```
public static Color getSkyBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSlateBlue() {#getSlateBlue--}
```
public static Color getSlateBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSlateGray() {#getSlateGray--}
```
public static Color getSlateGray()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSnow() {#getSnow--}
```
public static Color getSnow()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSpringGreen() {#getSpringGreen--}
```
public static Color getSpringGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getSteelBlue() {#getSteelBlue--}
```
public static Color getSteelBlue()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTan() {#getTan--}
```
public static Color getTan()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTeal() {#getTeal--}
```
public static Color getTeal()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getThistle() {#getThistle--}
```
public static Color getThistle()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTomato() {#getTomato--}
```
public static Color getTomato()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTransparent() {#getTransparent--}
```
public static Color getTransparent()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getTurquoise() {#getTurquoise--}
```
public static Color getTurquoise()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getViolet() {#getViolet--}
```
public static Color getViolet()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getWheat() {#getWheat--}
```
public static Color getWheat()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getWhite() {#getWhite--}
```
public static Color getWhite()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getWhiteSmoke() {#getWhiteSmoke--}
```
public static Color getWhiteSmoke()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getYellow() {#getYellow--}
```
public static Color getYellow()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### getYellowGreen() {#getYellowGreen--}
```
public static Color getYellowGreen()
```


Hämta en systemdefinierad färg.

**Returns:**
[Color](../../com.aspose.cells/color) - A Color object representing a system-defined color.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar en hashkod för detta Color-objekt.

**Returns:**
int - Ett heltal som specificerar hash-koden för detta Color-objekt.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Anger om detta Color-objekt är oinitierat.

**Returns:**
boolean - Denna egenskap returnerar true om denna färg är oinitierad; annars false.
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


Hämtar 32-bitars ARGB-värdet för detta Color-objekt.

**Returns:**
int - 32-bitars ARGB-värdet för detta Color-objekt.
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

