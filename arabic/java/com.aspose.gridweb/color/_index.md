---
title: "Color"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل لونًا بصيغة ARGB (ألفا، أحمر، أخضر، أزرق)."
type: docs
url: /ar/java/com.aspose.gridweb/color/
---

**Inheritance:**
java.lang.Object
```
public class Color
```

يمثل لون ARGB (ألفا، أحمر، أخضر، أزرق).
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Color()](#Color--) | دالة الإنشاء |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | يفحص ما إذا كان الكائن المحدد كائنًا من نوع Color ومكافئًا لهذا الكائن. |
| [fromArgb(int argb)](#fromArgb-int-) | ينشئ كائنًا من نوع Color من قيمة ARGB ذات 32 بت. |
| [fromArgb(int red, int green, int blue)](#fromArgb-int-int-int-) | ينشئ كائنًا من نوع Color من قيم الألوان ذات 8 بت المحددة (red، green، و blue). |
| [fromArgb(int alpha, int red, int green, int blue)](#fromArgb-int-int-int-int-) | ينشئ كائنًا من نوع Color من القيم الأربعة لمكوّنات ARGB (alpha، red، green، و blue). |
| [getA()](#getA--) | يحصل على قيمة مكوّن alpha لهذا الكائن من نوع Color. |
| [getAliceBlue()](#getAliceBlue--) | احصل على لون معرف من النظام. |
| [getAntiqueWhite()](#getAntiqueWhite--) | احصل على لون معرف من النظام. |
| [getAqua()](#getAqua--) | احصل على لون معرف من النظام. |
| [getAquamarine()](#getAquamarine--) | احصل على لون معرف من النظام. |
| [getAzure()](#getAzure--) | احصل على لون معرف من النظام. |
| [getB()](#getB--) | يحصل على قيمة مكوّن blue لهذا الكائن من نوع Color. |
| [getBeige()](#getBeige--) | احصل على لون معرف من النظام. |
| [getBisque()](#getBisque--) | احصل على لون معرف من النظام. |
| [getBlack()](#getBlack--) | احصل على لون معرف من النظام. |
| [getBlanchedAlmond()](#getBlanchedAlmond--) | احصل على لون معرف من النظام. |
| [getBlue()](#getBlue--) | احصل على لون معرف من النظام. |
| [getBlueViolet()](#getBlueViolet--) | احصل على لون معرف من النظام. |
| [getBrown()](#getBrown--) | احصل على لون معرف من النظام. |
| [getBurlyWood()](#getBurlyWood--) | احصل على لون معرف من النظام. |
| [getCadetBlue()](#getCadetBlue--) | احصل على لون معرف من النظام. |
| [getChartreuse()](#getChartreuse--) | احصل على لون معرف من النظام. |
| [getChocolate()](#getChocolate--) | احصل على لون معرف من النظام. |
| [getClass()](#getClass--) |  |
| [getCoral()](#getCoral--) | احصل على لون معرف من النظام. |
| [getCornflowerBlue()](#getCornflowerBlue--) | احصل على لون معرف من النظام. |
| [getCornsilk()](#getCornsilk--) | احصل على لون معرف من النظام. |
| [getCrimson()](#getCrimson--) | احصل على لون معرف من النظام. |
| [getCyan()](#getCyan--) | احصل على لون معرف من النظام. |
| [getDarkBlue()](#getDarkBlue--) | احصل على لون معرف من النظام. |
| [getDarkCyan()](#getDarkCyan--) | احصل على لون معرف من النظام. |
| [getDarkGoldenrod()](#getDarkGoldenrod--) | احصل على لون معرف من النظام. |
| [getDarkGray()](#getDarkGray--) | احصل على لون معرف من النظام. |
| [getDarkGreen()](#getDarkGreen--) | احصل على لون معرف من النظام. |
| [getDarkKhaki()](#getDarkKhaki--) | احصل على لون معرف من النظام. |
| [getDarkMagenta()](#getDarkMagenta--) | احصل على لون معرف من النظام. |
| [getDarkOliveGreen()](#getDarkOliveGreen--) | احصل على لون معرف من النظام. |
| [getDarkOrange()](#getDarkOrange--) | احصل على لون معرف من النظام. |
| [getDarkOrchid()](#getDarkOrchid--) | احصل على لون معرف من النظام. |
| [getDarkRed()](#getDarkRed--) | احصل على لون معرف من النظام. |
| [getDarkSalmon()](#getDarkSalmon--) | احصل على لون معرف من النظام. |
| [getDarkSeaGreen()](#getDarkSeaGreen--) | احصل على لون معرف من النظام. |
| [getDarkSlateBlue()](#getDarkSlateBlue--) | احصل على لون معرف من النظام. |
| [getDarkSlateGray()](#getDarkSlateGray--) | احصل على لون معرف من النظام. |
| [getDarkTurquoise()](#getDarkTurquoise--) | احصل على لون معرف من النظام. |
| [getDarkViolet()](#getDarkViolet--) | احصل على لون معرف من النظام. |
| [getDeepPink()](#getDeepPink--) | احصل على لون معرف من النظام. |
| [getDeepSkyBlue()](#getDeepSkyBlue--) | احصل على لون معرف من النظام. |
| [getDimGray()](#getDimGray--) | احصل على لون معرف من النظام. |
| [getDodgerBlue()](#getDodgerBlue--) | احصل على لون معرف من النظام. |
| [getEmpty()](#getEmpty--) | احصل على لون فارغ معرف من النظام. |
| [getFirebrick()](#getFirebrick--) | احصل على لون معرف من النظام. |
| [getFloralWhite()](#getFloralWhite--) | احصل على لون معرف من النظام. |
| [getForestGreen()](#getForestGreen--) | احصل على لون معرف من النظام. |
| [getFuchsia()](#getFuchsia--) | احصل على لون معرف من النظام. |
| [getG()](#getG--) | يحصل على قيمة مكوّن green لهذا الكائن من نوع Color. |
| [getGainsboro()](#getGainsboro--) | احصل على لون معرف من النظام. |
| [getGhostWhite()](#getGhostWhite--) | احصل على لون معرف من النظام. |
| [getGold()](#getGold--) | احصل على لون معرف من النظام. |
| [getGoldenrod()](#getGoldenrod--) | احصل على لون معرف من النظام. |
| [getGray()](#getGray--) | احصل على لون معرف من النظام. |
| [getGreen()](#getGreen--) | احصل على لون معرف من النظام. |
| [getGreenYellow()](#getGreenYellow--) | احصل على لون معرف من النظام. |
| [getHoneydew()](#getHoneydew--) | احصل على لون معرف من النظام. |
| [getHotPink()](#getHotPink--) | احصل على لون معرف من النظام. |
| [getIndianRed()](#getIndianRed--) | احصل على لون معرف من النظام. |
| [getIndigo()](#getIndigo--) | احصل على لون معرف من النظام. |
| [getIvory()](#getIvory--) | احصل على لون معرف من النظام. |
| [getKhaki()](#getKhaki--) | احصل على لون معرف من النظام. |
| [getLavender()](#getLavender--) | احصل على لون معرف من النظام. |
| [getLavenderBlush()](#getLavenderBlush--) | احصل على لون معرف من النظام. |
| [getLawnGreen()](#getLawnGreen--) | احصل على لون معرف من النظام. |
| [getLemonChiffon()](#getLemonChiffon--) | احصل على لون معرف من النظام. |
| [getLightBlue()](#getLightBlue--) | احصل على لون معرف من النظام. |
| [getLightCoral()](#getLightCoral--) | احصل على لون معرف من النظام. |
| [getLightCyan()](#getLightCyan--) | احصل على لون معرف من النظام. |
| [getLightGoldenrodYellow()](#getLightGoldenrodYellow--) | احصل على لون معرف من النظام. |
| [getLightGray()](#getLightGray--) | احصل على لون معرف من النظام. |
| [getLightGreen()](#getLightGreen--) | احصل على لون معرف من النظام. |
| [getLightPink()](#getLightPink--) | احصل على لون معرف من النظام. |
| [getLightSalmon()](#getLightSalmon--) | احصل على لون معرف من النظام. |
| [getLightSeaGreen()](#getLightSeaGreen--) | احصل على لون معرف من النظام. |
| [getLightSkyBlue()](#getLightSkyBlue--) | احصل على لون معرف من النظام. |
| [getLightSlateGray()](#getLightSlateGray--) | احصل على لون معرف من النظام. |
| [getLightSteelBlue()](#getLightSteelBlue--) | احصل على لون معرف من النظام. |
| [getLightYellow()](#getLightYellow--) | احصل على لون معرف من النظام. |
| [getLime()](#getLime--) | احصل على لون معرف من النظام. |
| [getLimeGreen()](#getLimeGreen--) | احصل على لون معرف من النظام. |
| [getLinen()](#getLinen--) | احصل على لون معرف من النظام. |
| [getMagenta()](#getMagenta--) | احصل على لون معرف من النظام. |
| [getMaroon()](#getMaroon--) | احصل على لون معرف من النظام. |
| [getMediumAquamarine()](#getMediumAquamarine--) | احصل على لون معرف من النظام. |
| [getMediumBlue()](#getMediumBlue--) | احصل على لون معرف من النظام. |
| [getMediumOrchid()](#getMediumOrchid--) | احصل على لون معرف من النظام. |
| [getMediumPurple()](#getMediumPurple--) | احصل على لون معرف من النظام. |
| [getMediumSeaGreen()](#getMediumSeaGreen--) | احصل على لون معرف من النظام. |
| [getMediumSlateBlue()](#getMediumSlateBlue--) | احصل على لون معرف من النظام. |
| [getMediumSpringGreen()](#getMediumSpringGreen--) | احصل على لون معرف من النظام. |
| [getMediumTurquoise()](#getMediumTurquoise--) | احصل على لون معرف من النظام. |
| [getMediumVioletRed()](#getMediumVioletRed--) | احصل على لون معرف من النظام. |
| [getMidnightBlue()](#getMidnightBlue--) | احصل على لون معرف من النظام. |
| [getMintCream()](#getMintCream--) | احصل على لون معرف من النظام. |
| [getMistyRose()](#getMistyRose--) | احصل على لون معرف من النظام. |
| [getMoccasin()](#getMoccasin--) | احصل على لون معرف من النظام. |
| [getNavajoWhite()](#getNavajoWhite--) | احصل على لون معرف من النظام. |
| [getNavy()](#getNavy--) | احصل على لون معرف من النظام. |
| [getOldLace()](#getOldLace--) | احصل على لون معرف من النظام. |
| [getOlive()](#getOlive--) | احصل على لون معرف من النظام. |
| [getOliveDrab()](#getOliveDrab--) | احصل على لون معرف من النظام. |
| [getOrange()](#getOrange--) | احصل على لون معرف من النظام. |
| [getOrangeRed()](#getOrangeRed--) | احصل على لون معرف من النظام. |
| [getOrchid()](#getOrchid--) | احصل على لون معرف من النظام. |
| [getPaleGoldenrod()](#getPaleGoldenrod--) | احصل على لون معرف من النظام. |
| [getPaleGreen()](#getPaleGreen--) | احصل على لون معرف من النظام. |
| [getPaleTurquoise()](#getPaleTurquoise--) | احصل على لون معرف من النظام. |
| [getPaleVioletRed()](#getPaleVioletRed--) | احصل على لون معرف من النظام. |
| [getPapayaWhip()](#getPapayaWhip--) | احصل على لون معرف من النظام. |
| [getPeachPuff()](#getPeachPuff--) | احصل على لون معرف من النظام. |
| [getPeru()](#getPeru--) | احصل على لون معرف من النظام. |
| [getPink()](#getPink--) | احصل على لون معرف من النظام. |
| [getPlum()](#getPlum--) | احصل على لون معرف من النظام. |
| [getPowderBlue()](#getPowderBlue--) | احصل على لون معرف من النظام. |
| [getPurple()](#getPurple--) | احصل على لون معرف من النظام. |
| [getR()](#getR--) | يحصل على قيمة مكوّن red لهذا الكائن من نوع Color. |
| [getRed()](#getRed--) | احصل على لون معرف من النظام. |
| [getRosyBrown()](#getRosyBrown--) | احصل على لون معرف من النظام. |
| [getRoyalBlue()](#getRoyalBlue--) | احصل على لون معرف من النظام. |
| [getSaddleBrown()](#getSaddleBrown--) | احصل على لون معرف من النظام. |
| [getSalmon()](#getSalmon--) | احصل على لون معرف من النظام. |
| [getSandyBrown()](#getSandyBrown--) | احصل على لون معرف من النظام. |
| [getSeaGreen()](#getSeaGreen--) | احصل على لون معرف من النظام. |
| [getSeaShell()](#getSeaShell--) | احصل على لون معرف من النظام. |
| [getSienna()](#getSienna--) | احصل على لون معرف من النظام. |
| [getSilver()](#getSilver--) | احصل على لون معرف من النظام. |
| [getSkyBlue()](#getSkyBlue--) | احصل على لون معرف من النظام. |
| [getSlateBlue()](#getSlateBlue--) | احصل على لون معرف من النظام. |
| [getSlateGray()](#getSlateGray--) | احصل على لون معرف من النظام. |
| [getSnow()](#getSnow--) | احصل على لون معرف من النظام. |
| [getSpringGreen()](#getSpringGreen--) | احصل على لون معرف من النظام. |
| [getSteelBlue()](#getSteelBlue--) | احصل على لون معرف من النظام. |
| [getTan()](#getTan--) | احصل على لون معرف من النظام. |
| [getTeal()](#getTeal--) | احصل على لون معرف من النظام. |
| [getThistle()](#getThistle--) | احصل على لون معرف من النظام. |
| [getTomato()](#getTomato--) | احصل على لون معرف من النظام. |
| [getTransparent()](#getTransparent--) | احصل على لون معرف من النظام. |
| [getTurquoise()](#getTurquoise--) | احصل على لون معرف من النظام. |
| [getViolet()](#getViolet--) | احصل على لون معرف من النظام. |
| [getWheat()](#getWheat--) | احصل على لون معرف من النظام. |
| [getWhite()](#getWhite--) | احصل على لون معرف من النظام. |
| [getWhiteSmoke()](#getWhiteSmoke--) | احصل على لون معرف من النظام. |
| [getYellow()](#getYellow--) | احصل على لون معرف من النظام. |
| [getYellowGreen()](#getYellowGreen--) | احصل على لون معرف من النظام. |
| [hashCode()](#hashCode--) | يرجع رمز تجزئة لهذا الكائن من نوع Color. |
| [isEmpty()](#isEmpty--) | يحدد ما إذا كان هذا الكائن من نوع Color غير مبدئ. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toArgb()](#toArgb--) | يحصل على قيمة ARGB ذات 32 بت لهذا الكائن من نوع Color. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Color() {#Color--}
```
public Color()
```


دالة الإنشاء

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يفحص ما إذا كان الكائن المحدد كائنًا من نوع Color ومكافئًا لهذا الكائن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن للاختبار. |

**Returns:**
boolean - true إذا كان obj كائنًا من نوع Color ومكافئًا لهذا الكائن من نوع Color؛ وإلا false.
### fromArgb(int argb) {#fromArgb-int-}
```
public static Color fromArgb(int argb)
```


ينشئ كائنًا من نوع Color من قيمة ARGB ذات 32 بت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| argb | int | قيمة تحدد قيمة ARGB ذات 32 بت. |

**Returns:**
[Color](../../com.aspose.gridweb/color) - The Color object that this method creates.
### fromArgb(int red, int green, int blue) {#fromArgb-int-int-int-}
```
public static Color fromArgb(int red, int green, int blue)
```


ينشئ كائنًا من نوع Color من قيم الألوان ذات 8 بت المحددة (red، green، و blue). قيمة alpha هي ضمنيًا 255 (معتمة بالكامل). على الرغم من أن هذه الطريقة تسمح بتمرير قيمة 32 بت لكل مكوّن لون، فإن قيمة كل مكوّن محدودة بـ 8 بت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| red | int | قيمة مكوّن red للكائن الجديد من نوع Color. القيم الصالحة هي من 0 إلى 255. |
| green | int | قيمة مكوّن green للكائن الجديد من نوع Color. القيم الصالحة هي من 0 إلى 255. |
| blue | int | قيمة مكوّن blue للكائن الجديد من نوع Color. القيم الصالحة هي من 0 إلى 255. |

**Returns:**
[Color](../../com.aspose.gridweb/color) - The Color object that this method creates.
### fromArgb(int alpha, int red, int green, int blue) {#fromArgb-int-int-int-int-}
```
public static Color fromArgb(int alpha, int red, int green, int blue)
```


ينشئ كائنًا من نوع Color من القيم الأربعة لمكوّنات ARGB (alpha، red، green، و blue). على الرغم من أن هذه الطريقة تسمح بتمرير قيمة 32 بت لكل مكوّن، فإن قيمة كل مكوّن محدودة بـ 8 بت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| alpha | int | المكوّن alpha. القيم الصالحة هي من 0 إلى 255. |
| red | int | المكوّن red. القيم الصالحة هي من 0 إلى 255. |
| green | int | المكوّن green. القيم الصالحة هي من 0 إلى 255. |
| blue | int | المكوّن blue. القيم الصالحة هي من 0 إلى 255. |

**Returns:**
[Color](../../com.aspose.gridweb/color) - The Color object that this method creates.
### getA() {#getA--}
```
public byte getA()
```


يحصل على قيمة مكوّن alpha لهذا الكائن من نوع Color.

**Returns:**
byte - قيمة المكوّن alpha لهذا الكائن Color.
### getAliceBlue() {#getAliceBlue--}
```
public static Color getAliceBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getAntiqueWhite() {#getAntiqueWhite--}
```
public static Color getAntiqueWhite()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getAqua() {#getAqua--}
```
public static Color getAqua()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getAquamarine() {#getAquamarine--}
```
public static Color getAquamarine()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getAzure() {#getAzure--}
```
public static Color getAzure()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getB() {#getB--}
```
public byte getB()
```


يحصل على قيمة مكوّن blue لهذا الكائن من نوع Color.

**Returns:**
byte - قيمة المكوّن blue لهذا الكائن Color.
### getBeige() {#getBeige--}
```
public static Color getBeige()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBisque() {#getBisque--}
```
public static Color getBisque()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBlack() {#getBlack--}
```
public static Color getBlack()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBlanchedAlmond() {#getBlanchedAlmond--}
```
public static Color getBlanchedAlmond()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBlue() {#getBlue--}
```
public static Color getBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBlueViolet() {#getBlueViolet--}
```
public static Color getBlueViolet()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBrown() {#getBrown--}
```
public static Color getBrown()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBurlyWood() {#getBurlyWood--}
```
public static Color getBurlyWood()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCadetBlue() {#getCadetBlue--}
```
public static Color getCadetBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getChartreuse() {#getChartreuse--}
```
public static Color getChartreuse()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getChocolate() {#getChocolate--}
```
public static Color getChocolate()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
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


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCornflowerBlue() {#getCornflowerBlue--}
```
public static Color getCornflowerBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCornsilk() {#getCornsilk--}
```
public static Color getCornsilk()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCrimson() {#getCrimson--}
```
public static Color getCrimson()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCyan() {#getCyan--}
```
public static Color getCyan()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkBlue() {#getDarkBlue--}
```
public static Color getDarkBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkCyan() {#getDarkCyan--}
```
public static Color getDarkCyan()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkGoldenrod() {#getDarkGoldenrod--}
```
public static Color getDarkGoldenrod()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkGray() {#getDarkGray--}
```
public static Color getDarkGray()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkGreen() {#getDarkGreen--}
```
public static Color getDarkGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkKhaki() {#getDarkKhaki--}
```
public static Color getDarkKhaki()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkMagenta() {#getDarkMagenta--}
```
public static Color getDarkMagenta()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkOliveGreen() {#getDarkOliveGreen--}
```
public static Color getDarkOliveGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkOrange() {#getDarkOrange--}
```
public static Color getDarkOrange()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkOrchid() {#getDarkOrchid--}
```
public static Color getDarkOrchid()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkRed() {#getDarkRed--}
```
public static Color getDarkRed()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkSalmon() {#getDarkSalmon--}
```
public static Color getDarkSalmon()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkSeaGreen() {#getDarkSeaGreen--}
```
public static Color getDarkSeaGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkSlateBlue() {#getDarkSlateBlue--}
```
public static Color getDarkSlateBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkSlateGray() {#getDarkSlateGray--}
```
public static Color getDarkSlateGray()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkTurquoise() {#getDarkTurquoise--}
```
public static Color getDarkTurquoise()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkViolet() {#getDarkViolet--}
```
public static Color getDarkViolet()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDeepPink() {#getDeepPink--}
```
public static Color getDeepPink()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDeepSkyBlue() {#getDeepSkyBlue--}
```
public static Color getDeepSkyBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDimGray() {#getDimGray--}
```
public static Color getDimGray()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDodgerBlue() {#getDodgerBlue--}
```
public static Color getDodgerBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getEmpty() {#getEmpty--}
```
public static Color getEmpty()
```


احصل على لون فارغ معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getFirebrick() {#getFirebrick--}
```
public static Color getFirebrick()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getFloralWhite() {#getFloralWhite--}
```
public static Color getFloralWhite()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getForestGreen() {#getForestGreen--}
```
public static Color getForestGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getFuchsia() {#getFuchsia--}
```
public static Color getFuchsia()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getG() {#getG--}
```
public byte getG()
```


يحصل على قيمة مكوّن green لهذا الكائن من نوع Color.

**Returns:**
byte - قيمة المكوّن green لهذا الكائن Color.
### getGainsboro() {#getGainsboro--}
```
public static Color getGainsboro()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGhostWhite() {#getGhostWhite--}
```
public static Color getGhostWhite()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGold() {#getGold--}
```
public static Color getGold()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGoldenrod() {#getGoldenrod--}
```
public static Color getGoldenrod()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGray() {#getGray--}
```
public static Color getGray()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGreen() {#getGreen--}
```
public static Color getGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGreenYellow() {#getGreenYellow--}
```
public static Color getGreenYellow()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getHoneydew() {#getHoneydew--}
```
public static Color getHoneydew()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getHotPink() {#getHotPink--}
```
public static Color getHotPink()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getIndianRed() {#getIndianRed--}
```
public static Color getIndianRed()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getIndigo() {#getIndigo--}
```
public static Color getIndigo()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getIvory() {#getIvory--}
```
public static Color getIvory()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getKhaki() {#getKhaki--}
```
public static Color getKhaki()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLavender() {#getLavender--}
```
public static Color getLavender()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLavenderBlush() {#getLavenderBlush--}
```
public static Color getLavenderBlush()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLawnGreen() {#getLawnGreen--}
```
public static Color getLawnGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLemonChiffon() {#getLemonChiffon--}
```
public static Color getLemonChiffon()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightBlue() {#getLightBlue--}
```
public static Color getLightBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightCoral() {#getLightCoral--}
```
public static Color getLightCoral()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightCyan() {#getLightCyan--}
```
public static Color getLightCyan()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightGoldenrodYellow() {#getLightGoldenrodYellow--}
```
public static Color getLightGoldenrodYellow()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightGray() {#getLightGray--}
```
public static Color getLightGray()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightGreen() {#getLightGreen--}
```
public static Color getLightGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightPink() {#getLightPink--}
```
public static Color getLightPink()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSalmon() {#getLightSalmon--}
```
public static Color getLightSalmon()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSeaGreen() {#getLightSeaGreen--}
```
public static Color getLightSeaGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSkyBlue() {#getLightSkyBlue--}
```
public static Color getLightSkyBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSlateGray() {#getLightSlateGray--}
```
public static Color getLightSlateGray()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSteelBlue() {#getLightSteelBlue--}
```
public static Color getLightSteelBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightYellow() {#getLightYellow--}
```
public static Color getLightYellow()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLime() {#getLime--}
```
public static Color getLime()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLimeGreen() {#getLimeGreen--}
```
public static Color getLimeGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLinen() {#getLinen--}
```
public static Color getLinen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMagenta() {#getMagenta--}
```
public static Color getMagenta()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMaroon() {#getMaroon--}
```
public static Color getMaroon()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumAquamarine() {#getMediumAquamarine--}
```
public static Color getMediumAquamarine()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumBlue() {#getMediumBlue--}
```
public static Color getMediumBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumOrchid() {#getMediumOrchid--}
```
public static Color getMediumOrchid()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumPurple() {#getMediumPurple--}
```
public static Color getMediumPurple()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumSeaGreen() {#getMediumSeaGreen--}
```
public static Color getMediumSeaGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumSlateBlue() {#getMediumSlateBlue--}
```
public static Color getMediumSlateBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumSpringGreen() {#getMediumSpringGreen--}
```
public static Color getMediumSpringGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumTurquoise() {#getMediumTurquoise--}
```
public static Color getMediumTurquoise()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumVioletRed() {#getMediumVioletRed--}
```
public static Color getMediumVioletRed()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMidnightBlue() {#getMidnightBlue--}
```
public static Color getMidnightBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMintCream() {#getMintCream--}
```
public static Color getMintCream()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMistyRose() {#getMistyRose--}
```
public static Color getMistyRose()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMoccasin() {#getMoccasin--}
```
public static Color getMoccasin()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getNavajoWhite() {#getNavajoWhite--}
```
public static Color getNavajoWhite()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getNavy() {#getNavy--}
```
public static Color getNavy()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOldLace() {#getOldLace--}
```
public static Color getOldLace()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOlive() {#getOlive--}
```
public static Color getOlive()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOliveDrab() {#getOliveDrab--}
```
public static Color getOliveDrab()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOrange() {#getOrange--}
```
public static Color getOrange()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOrangeRed() {#getOrangeRed--}
```
public static Color getOrangeRed()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOrchid() {#getOrchid--}
```
public static Color getOrchid()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPaleGoldenrod() {#getPaleGoldenrod--}
```
public static Color getPaleGoldenrod()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPaleGreen() {#getPaleGreen--}
```
public static Color getPaleGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPaleTurquoise() {#getPaleTurquoise--}
```
public static Color getPaleTurquoise()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPaleVioletRed() {#getPaleVioletRed--}
```
public static Color getPaleVioletRed()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPapayaWhip() {#getPapayaWhip--}
```
public static Color getPapayaWhip()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPeachPuff() {#getPeachPuff--}
```
public static Color getPeachPuff()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPeru() {#getPeru--}
```
public static Color getPeru()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPink() {#getPink--}
```
public static Color getPink()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPlum() {#getPlum--}
```
public static Color getPlum()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPowderBlue() {#getPowderBlue--}
```
public static Color getPowderBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPurple() {#getPurple--}
```
public static Color getPurple()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getR() {#getR--}
```
public byte getR()
```


يحصل على قيمة مكوّن red لهذا الكائن من نوع Color.

**Returns:**
byte - قيمة المكوّن red لهذا الكائن Color.
### getRed() {#getRed--}
```
public static Color getRed()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getRosyBrown() {#getRosyBrown--}
```
public static Color getRosyBrown()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getRoyalBlue() {#getRoyalBlue--}
```
public static Color getRoyalBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSaddleBrown() {#getSaddleBrown--}
```
public static Color getSaddleBrown()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSalmon() {#getSalmon--}
```
public static Color getSalmon()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSandyBrown() {#getSandyBrown--}
```
public static Color getSandyBrown()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSeaGreen() {#getSeaGreen--}
```
public static Color getSeaGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSeaShell() {#getSeaShell--}
```
public static Color getSeaShell()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSienna() {#getSienna--}
```
public static Color getSienna()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSilver() {#getSilver--}
```
public static Color getSilver()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSkyBlue() {#getSkyBlue--}
```
public static Color getSkyBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSlateBlue() {#getSlateBlue--}
```
public static Color getSlateBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSlateGray() {#getSlateGray--}
```
public static Color getSlateGray()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSnow() {#getSnow--}
```
public static Color getSnow()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSpringGreen() {#getSpringGreen--}
```
public static Color getSpringGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSteelBlue() {#getSteelBlue--}
```
public static Color getSteelBlue()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTan() {#getTan--}
```
public static Color getTan()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTeal() {#getTeal--}
```
public static Color getTeal()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getThistle() {#getThistle--}
```
public static Color getThistle()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTomato() {#getTomato--}
```
public static Color getTomato()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTransparent() {#getTransparent--}
```
public static Color getTransparent()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTurquoise() {#getTurquoise--}
```
public static Color getTurquoise()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getViolet() {#getViolet--}
```
public static Color getViolet()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getWheat() {#getWheat--}
```
public static Color getWheat()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getWhite() {#getWhite--}
```
public static Color getWhite()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getWhiteSmoke() {#getWhiteSmoke--}
```
public static Color getWhiteSmoke()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getYellow() {#getYellow--}
```
public static Color getYellow()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getYellowGreen() {#getYellowGreen--}
```
public static Color getYellowGreen()
```


احصل على لون معرف من النظام.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يرجع رمز تجزئة لهذا الكائن من نوع Color.

**Returns:**
int - قيمة عددية صحيحة تحدد رمز التجزئة لهذا الكائن Color.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


يحدد ما إذا كان هذا الكائن من نوع Color غير مبدئ.

**Returns:**
boolean - تُعيد هذه الخاصية true إذا كان هذا اللون غير مهيأ؛ وإلا false.
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


يحصل على قيمة ARGB ذات 32 بت لهذا الكائن من نوع Color.

**Returns:**
int - قيمة ARGB ذات 32 بت لهذا الكائن Color.
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

