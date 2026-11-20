---
title: "Color"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет цвет в формате ARGB (альфа, красный, зелёный, синий)."
type: docs
url: /ru/java/com.aspose.gridweb/color/
---

**Inheritance:**
java.lang.Object
```
public class Color
```

Представляет цвет ARGB (альфа, красный, зелёный, синий).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Color()](#Color--) | конструктор функции |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Проверяет, является ли указанный объект объектом Color и эквивалентен ли он этому объекту. |
| [fromArgb(int argb)](#fromArgb-int-) | Создаёт объект Color из 32‑битного значения ARGB. |
| [fromArgb(int red, int green, int blue)](#fromArgb-int-int-int-) | Создаёт объект Color из указанных 8‑битных значений цветов (красный, зелёный и синий). |
| [fromArgb(int alpha, int red, int green, int blue)](#fromArgb-int-int-int-int-) | Создаёт объект Color из четырёх значений компонентов ARGB (альфа, красный, зелёный и синий). |
| [getA()](#getA--) | Получает значение альфа‑компоненты этого объекта Color. |
| [getAliceBlue()](#getAliceBlue--) | Получить системно‑определённый цвет. |
| [getAntiqueWhite()](#getAntiqueWhite--) | Получить системно‑определённый цвет. |
| [getAqua()](#getAqua--) | Получить системно‑определённый цвет. |
| [getAquamarine()](#getAquamarine--) | Получить системно‑определённый цвет. |
| [getAzure()](#getAzure--) | Получить системно‑определённый цвет. |
| [getB()](#getB--) | Получает значение синего компонента этого объекта Color. |
| [getBeige()](#getBeige--) | Получить системно‑определённый цвет. |
| [getBisque()](#getBisque--) | Получить системно‑определённый цвет. |
| [getBlack()](#getBlack--) | Получить системно‑определённый цвет. |
| [getBlanchedAlmond()](#getBlanchedAlmond--) | Получить системно‑определённый цвет. |
| [getBlue()](#getBlue--) | Получить системно‑определённый цвет. |
| [getBlueViolet()](#getBlueViolet--) | Получить системно‑определённый цвет. |
| [getBrown()](#getBrown--) | Получить системно‑определённый цвет. |
| [getBurlyWood()](#getBurlyWood--) | Получить системно‑определённый цвет. |
| [getCadetBlue()](#getCadetBlue--) | Получить системно‑определённый цвет. |
| [getChartreuse()](#getChartreuse--) | Получить системно‑определённый цвет. |
| [getChocolate()](#getChocolate--) | Получить системно‑определённый цвет. |
| [getClass()](#getClass--) |  |
| [getCoral()](#getCoral--) | Получить системно‑определённый цвет. |
| [getCornflowerBlue()](#getCornflowerBlue--) | Получить системно‑определённый цвет. |
| [getCornsilk()](#getCornsilk--) | Получить системно‑определённый цвет. |
| [getCrimson()](#getCrimson--) | Получить системно‑определённый цвет. |
| [getCyan()](#getCyan--) | Получить системно‑определённый цвет. |
| [getDarkBlue()](#getDarkBlue--) | Получить системно‑определённый цвет. |
| [getDarkCyan()](#getDarkCyan--) | Получить системно‑определённый цвет. |
| [getDarkGoldenrod()](#getDarkGoldenrod--) | Получить системно‑определённый цвет. |
| [getDarkGray()](#getDarkGray--) | Получить системно‑определённый цвет. |
| [getDarkGreen()](#getDarkGreen--) | Получить системно‑определённый цвет. |
| [getDarkKhaki()](#getDarkKhaki--) | Получить системно‑определённый цвет. |
| [getDarkMagenta()](#getDarkMagenta--) | Получить системно‑определённый цвет. |
| [getDarkOliveGreen()](#getDarkOliveGreen--) | Получить системно‑определённый цвет. |
| [getDarkOrange()](#getDarkOrange--) | Получить системно‑определённый цвет. |
| [getDarkOrchid()](#getDarkOrchid--) | Получить системно‑определённый цвет. |
| [getDarkRed()](#getDarkRed--) | Получить системно‑определённый цвет. |
| [getDarkSalmon()](#getDarkSalmon--) | Получить системно‑определённый цвет. |
| [getDarkSeaGreen()](#getDarkSeaGreen--) | Получить системно‑определённый цвет. |
| [getDarkSlateBlue()](#getDarkSlateBlue--) | Получить системно‑определённый цвет. |
| [getDarkSlateGray()](#getDarkSlateGray--) | Получить системно‑определённый цвет. |
| [getDarkTurquoise()](#getDarkTurquoise--) | Получить системно‑определённый цвет. |
| [getDarkViolet()](#getDarkViolet--) | Получить системно‑определённый цвет. |
| [getDeepPink()](#getDeepPink--) | Получить системно‑определённый цвет. |
| [getDeepSkyBlue()](#getDeepSkyBlue--) | Получить системно‑определённый цвет. |
| [getDimGray()](#getDimGray--) | Получить системно‑определённый цвет. |
| [getDodgerBlue()](#getDodgerBlue--) | Получить системно‑определённый цвет. |
| [getEmpty()](#getEmpty--) | Получить системно‑определённый пустой цвет. |
| [getFirebrick()](#getFirebrick--) | Получить системно‑определённый цвет. |
| [getFloralWhite()](#getFloralWhite--) | Получить системно‑определённый цвет. |
| [getForestGreen()](#getForestGreen--) | Получить системно‑определённый цвет. |
| [getFuchsia()](#getFuchsia--) | Получить системно‑определённый цвет. |
| [getG()](#getG--) | Получает значение зелёного компонента этого объекта Color. |
| [getGainsboro()](#getGainsboro--) | Получить системно‑определённый цвет. |
| [getGhostWhite()](#getGhostWhite--) | Получить системно‑определённый цвет. |
| [getGold()](#getGold--) | Получить системно‑определённый цвет. |
| [getGoldenrod()](#getGoldenrod--) | Получить системно‑определённый цвет. |
| [getGray()](#getGray--) | Получить системно‑определённый цвет. |
| [getGreen()](#getGreen--) | Получить системно‑определённый цвет. |
| [getGreenYellow()](#getGreenYellow--) | Получить системно‑определённый цвет. |
| [getHoneydew()](#getHoneydew--) | Получить системно‑определённый цвет. |
| [getHotPink()](#getHotPink--) | Получить системно‑определённый цвет. |
| [getIndianRed()](#getIndianRed--) | Получить системно‑определённый цвет. |
| [getIndigo()](#getIndigo--) | Получить системно‑определённый цвет. |
| [getIvory()](#getIvory--) | Получить системно‑определённый цвет. |
| [getKhaki()](#getKhaki--) | Получить системно‑определённый цвет. |
| [getLavender()](#getLavender--) | Получить системно‑определённый цвет. |
| [getLavenderBlush()](#getLavenderBlush--) | Получить системно‑определённый цвет. |
| [getLawnGreen()](#getLawnGreen--) | Получить системно‑определённый цвет. |
| [getLemonChiffon()](#getLemonChiffon--) | Получить системно‑определённый цвет. |
| [getLightBlue()](#getLightBlue--) | Получить системно‑определённый цвет. |
| [getLightCoral()](#getLightCoral--) | Получить системно‑определённый цвет. |
| [getLightCyan()](#getLightCyan--) | Получить системно‑определённый цвет. |
| [getLightGoldenrodYellow()](#getLightGoldenrodYellow--) | Получить системно‑определённый цвет. |
| [getLightGray()](#getLightGray--) | Получить системно‑определённый цвет. |
| [getLightGreen()](#getLightGreen--) | Получить системно‑определённый цвет. |
| [getLightPink()](#getLightPink--) | Получить системно‑определённый цвет. |
| [getLightSalmon()](#getLightSalmon--) | Получить системно‑определённый цвет. |
| [getLightSeaGreen()](#getLightSeaGreen--) | Получить системно‑определённый цвет. |
| [getLightSkyBlue()](#getLightSkyBlue--) | Получить системно‑определённый цвет. |
| [getLightSlateGray()](#getLightSlateGray--) | Получить системно‑определённый цвет. |
| [getLightSteelBlue()](#getLightSteelBlue--) | Получить системно‑определённый цвет. |
| [getLightYellow()](#getLightYellow--) | Получить системно‑определённый цвет. |
| [getLime()](#getLime--) | Получить системно‑определённый цвет. |
| [getLimeGreen()](#getLimeGreen--) | Получить системно‑определённый цвет. |
| [getLinen()](#getLinen--) | Получить системно‑определённый цвет. |
| [getMagenta()](#getMagenta--) | Получить системно‑определённый цвет. |
| [getMaroon()](#getMaroon--) | Получить системно‑определённый цвет. |
| [getMediumAquamarine()](#getMediumAquamarine--) | Получить системно‑определённый цвет. |
| [getMediumBlue()](#getMediumBlue--) | Получить системно‑определённый цвет. |
| [getMediumOrchid()](#getMediumOrchid--) | Получить системно‑определённый цвет. |
| [getMediumPurple()](#getMediumPurple--) | Получить системно‑определённый цвет. |
| [getMediumSeaGreen()](#getMediumSeaGreen--) | Получить системно‑определённый цвет. |
| [getMediumSlateBlue()](#getMediumSlateBlue--) | Получить системно‑определённый цвет. |
| [getMediumSpringGreen()](#getMediumSpringGreen--) | Получить системно‑определённый цвет. |
| [getMediumTurquoise()](#getMediumTurquoise--) | Получить системно‑определённый цвет. |
| [getMediumVioletRed()](#getMediumVioletRed--) | Получить системно‑определённый цвет. |
| [getMidnightBlue()](#getMidnightBlue--) | Получить системно‑определённый цвет. |
| [getMintCream()](#getMintCream--) | Получить системно‑определённый цвет. |
| [getMistyRose()](#getMistyRose--) | Получить системно‑определённый цвет. |
| [getMoccasin()](#getMoccasin--) | Получить системно‑определённый цвет. |
| [getNavajoWhite()](#getNavajoWhite--) | Получить системно‑определённый цвет. |
| [getNavy()](#getNavy--) | Получить системно‑определённый цвет. |
| [getOldLace()](#getOldLace--) | Получить системно‑определённый цвет. |
| [getOlive()](#getOlive--) | Получить системно‑определённый цвет. |
| [getOliveDrab()](#getOliveDrab--) | Получить системно‑определённый цвет. |
| [getOrange()](#getOrange--) | Получить системно‑определённый цвет. |
| [getOrangeRed()](#getOrangeRed--) | Получить системно‑определённый цвет. |
| [getOrchid()](#getOrchid--) | Получить системно‑определённый цвет. |
| [getPaleGoldenrod()](#getPaleGoldenrod--) | Получить системно‑определённый цвет. |
| [getPaleGreen()](#getPaleGreen--) | Получить системно‑определённый цвет. |
| [getPaleTurquoise()](#getPaleTurquoise--) | Получить системно‑определённый цвет. |
| [getPaleVioletRed()](#getPaleVioletRed--) | Получить системно‑определённый цвет. |
| [getPapayaWhip()](#getPapayaWhip--) | Получить системно‑определённый цвет. |
| [getPeachPuff()](#getPeachPuff--) | Получить системно‑определённый цвет. |
| [getPeru()](#getPeru--) | Получить системно‑определённый цвет. |
| [getPink()](#getPink--) | Получить системно‑определённый цвет. |
| [getPlum()](#getPlum--) | Получить системно‑определённый цвет. |
| [getPowderBlue()](#getPowderBlue--) | Получить системно‑определённый цвет. |
| [getPurple()](#getPurple--) | Получить системно‑определённый цвет. |
| [getR()](#getR--) | Получает значение красного компонента этого объекта Color. |
| [getRed()](#getRed--) | Получить системно‑определённый цвет. |
| [getRosyBrown()](#getRosyBrown--) | Получить системно‑определённый цвет. |
| [getRoyalBlue()](#getRoyalBlue--) | Получить системно‑определённый цвет. |
| [getSaddleBrown()](#getSaddleBrown--) | Получить системно‑определённый цвет. |
| [getSalmon()](#getSalmon--) | Получить системно‑определённый цвет. |
| [getSandyBrown()](#getSandyBrown--) | Получить системно‑определённый цвет. |
| [getSeaGreen()](#getSeaGreen--) | Получить системно‑определённый цвет. |
| [getSeaShell()](#getSeaShell--) | Получить системно‑определённый цвет. |
| [getSienna()](#getSienna--) | Получить системно‑определённый цвет. |
| [getSilver()](#getSilver--) | Получить системно‑определённый цвет. |
| [getSkyBlue()](#getSkyBlue--) | Получить системно‑определённый цвет. |
| [getSlateBlue()](#getSlateBlue--) | Получить системно‑определённый цвет. |
| [getSlateGray()](#getSlateGray--) | Получить системно‑определённый цвет. |
| [getSnow()](#getSnow--) | Получить системно‑определённый цвет. |
| [getSpringGreen()](#getSpringGreen--) | Получить системно‑определённый цвет. |
| [getSteelBlue()](#getSteelBlue--) | Получить системно‑определённый цвет. |
| [getTan()](#getTan--) | Получить системно‑определённый цвет. |
| [getTeal()](#getTeal--) | Получить системно‑определённый цвет. |
| [getThistle()](#getThistle--) | Получить системно‑определённый цвет. |
| [getTomato()](#getTomato--) | Получить системно‑определённый цвет. |
| [getTransparent()](#getTransparent--) | Получить системно‑определённый цвет. |
| [getTurquoise()](#getTurquoise--) | Получить системно‑определённый цвет. |
| [getViolet()](#getViolet--) | Получить системно‑определённый цвет. |
| [getWheat()](#getWheat--) | Получить системно‑определённый цвет. |
| [getWhite()](#getWhite--) | Получить системно‑определённый цвет. |
| [getWhiteSmoke()](#getWhiteSmoke--) | Получить системно‑определённый цвет. |
| [getYellow()](#getYellow--) | Получить системно‑определённый цвет. |
| [getYellowGreen()](#getYellowGreen--) | Получить системно‑определённый цвет. |
| [hashCode()](#hashCode--) | Возвращает хеш‑код для этого объекта Color. |
| [isEmpty()](#isEmpty--) | Указывает, является ли этот объект Color неинициализированным. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toArgb()](#toArgb--) | Получает 32‑битное значение ARGB этого объекта Color. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Color() {#Color--}
```
public Color()
```


конструктор функции

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Проверяет, является ли указанный объект объектом Color и эквивалентен ли он этому объекту.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | Объект для тестирования. |

**Returns:**
boolean — true, если obj является объектом Color и эквивалентен этому объекту Color; иначе false.
### fromArgb(int argb) {#fromArgb-int-}
```
public static Color fromArgb(int argb)
```


Создаёт объект Color из 32‑битного значения ARGB.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| argb | int | Значение, задающее 32‑битное значение ARGB. |

**Returns:**
[Color](../../com.aspose.gridweb/color) - The Color object that this method creates.
### fromArgb(int red, int green, int blue) {#fromArgb-int-int-int-}
```
public static Color fromArgb(int red, int green, int blue)
```


Создаёт объект Color из указанных 8‑битных значений цветов (красный, зелёный и синий). Значение альфа подразумевается равным 255 (полностью непрозрачным). Хотя этот метод позволяет передавать 32‑битное значение для каждого цветового компонента, значение каждого компонента ограничено 8 битами.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| красный | int | Значение красного компонента нового объекта Color. Допустимые значения от 0 до 255. |
| зелёный | int | Значение зелёного компонента нового объекта Color. Допустимые значения от 0 до 255. |
| синий | int | Значение синего компонента нового объекта Color. Допустимые значения от 0 до 255. |

**Returns:**
[Color](../../com.aspose.gridweb/color) - The Color object that this method creates.
### fromArgb(int alpha, int red, int green, int blue) {#fromArgb-int-int-int-int-}
```
public static Color fromArgb(int alpha, int red, int green, int blue)
```


Создаёт объект Color из четырёх значений компонентов ARGB (альфа, красный, зелёный и синий). Хотя этот метод позволяет передавать 32‑битное значение для каждого компонента, значение каждого компонента ограничено 8 битами.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| альфа | int | Альфа‑компонент. Допустимые значения от 0 до 255. |
| красный | int | Красный компонент. Допустимые значения от 0 до 255. |
| зелёный | int | Зелёный компонент. Допустимые значения от 0 до 255. |
| синий | int | Синий компонент. Допустимые значения от 0 до 255. |

**Returns:**
[Color](../../com.aspose.gridweb/color) - The Color object that this method creates.
### getA() {#getA--}
```
public byte getA()
```


Получает значение альфа‑компоненты этого объекта Color.

**Returns:**
byte — значение альфа‑компонента этого объекта Color.
### getAliceBlue() {#getAliceBlue--}
```
public static Color getAliceBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getAntiqueWhite() {#getAntiqueWhite--}
```
public static Color getAntiqueWhite()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getAqua() {#getAqua--}
```
public static Color getAqua()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getAquamarine() {#getAquamarine--}
```
public static Color getAquamarine()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getAzure() {#getAzure--}
```
public static Color getAzure()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getB() {#getB--}
```
public byte getB()
```


Получает значение синего компонента этого объекта Color.

**Returns:**
byte — значение синего компонента этого объекта Color.
### getBeige() {#getBeige--}
```
public static Color getBeige()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBisque() {#getBisque--}
```
public static Color getBisque()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBlack() {#getBlack--}
```
public static Color getBlack()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBlanchedAlmond() {#getBlanchedAlmond--}
```
public static Color getBlanchedAlmond()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBlue() {#getBlue--}
```
public static Color getBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBlueViolet() {#getBlueViolet--}
```
public static Color getBlueViolet()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBrown() {#getBrown--}
```
public static Color getBrown()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getBurlyWood() {#getBurlyWood--}
```
public static Color getBurlyWood()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCadetBlue() {#getCadetBlue--}
```
public static Color getCadetBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getChartreuse() {#getChartreuse--}
```
public static Color getChartreuse()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getChocolate() {#getChocolate--}
```
public static Color getChocolate()
```


Получить системно‑определённый цвет.

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


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCornflowerBlue() {#getCornflowerBlue--}
```
public static Color getCornflowerBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCornsilk() {#getCornsilk--}
```
public static Color getCornsilk()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCrimson() {#getCrimson--}
```
public static Color getCrimson()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getCyan() {#getCyan--}
```
public static Color getCyan()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkBlue() {#getDarkBlue--}
```
public static Color getDarkBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkCyan() {#getDarkCyan--}
```
public static Color getDarkCyan()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkGoldenrod() {#getDarkGoldenrod--}
```
public static Color getDarkGoldenrod()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkGray() {#getDarkGray--}
```
public static Color getDarkGray()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkGreen() {#getDarkGreen--}
```
public static Color getDarkGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkKhaki() {#getDarkKhaki--}
```
public static Color getDarkKhaki()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkMagenta() {#getDarkMagenta--}
```
public static Color getDarkMagenta()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkOliveGreen() {#getDarkOliveGreen--}
```
public static Color getDarkOliveGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkOrange() {#getDarkOrange--}
```
public static Color getDarkOrange()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkOrchid() {#getDarkOrchid--}
```
public static Color getDarkOrchid()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkRed() {#getDarkRed--}
```
public static Color getDarkRed()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkSalmon() {#getDarkSalmon--}
```
public static Color getDarkSalmon()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkSeaGreen() {#getDarkSeaGreen--}
```
public static Color getDarkSeaGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkSlateBlue() {#getDarkSlateBlue--}
```
public static Color getDarkSlateBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkSlateGray() {#getDarkSlateGray--}
```
public static Color getDarkSlateGray()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkTurquoise() {#getDarkTurquoise--}
```
public static Color getDarkTurquoise()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDarkViolet() {#getDarkViolet--}
```
public static Color getDarkViolet()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDeepPink() {#getDeepPink--}
```
public static Color getDeepPink()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDeepSkyBlue() {#getDeepSkyBlue--}
```
public static Color getDeepSkyBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDimGray() {#getDimGray--}
```
public static Color getDimGray()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getDodgerBlue() {#getDodgerBlue--}
```
public static Color getDodgerBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getEmpty() {#getEmpty--}
```
public static Color getEmpty()
```


Получить системно‑определённый пустой цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getFirebrick() {#getFirebrick--}
```
public static Color getFirebrick()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getFloralWhite() {#getFloralWhite--}
```
public static Color getFloralWhite()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getForestGreen() {#getForestGreen--}
```
public static Color getForestGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getFuchsia() {#getFuchsia--}
```
public static Color getFuchsia()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getG() {#getG--}
```
public byte getG()
```


Получает значение зелёного компонента этого объекта Color.

**Returns:**
byte — значение зелёного компонента этого объекта Color.
### getGainsboro() {#getGainsboro--}
```
public static Color getGainsboro()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGhostWhite() {#getGhostWhite--}
```
public static Color getGhostWhite()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGold() {#getGold--}
```
public static Color getGold()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGoldenrod() {#getGoldenrod--}
```
public static Color getGoldenrod()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGray() {#getGray--}
```
public static Color getGray()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGreen() {#getGreen--}
```
public static Color getGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getGreenYellow() {#getGreenYellow--}
```
public static Color getGreenYellow()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getHoneydew() {#getHoneydew--}
```
public static Color getHoneydew()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getHotPink() {#getHotPink--}
```
public static Color getHotPink()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getIndianRed() {#getIndianRed--}
```
public static Color getIndianRed()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getIndigo() {#getIndigo--}
```
public static Color getIndigo()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getIvory() {#getIvory--}
```
public static Color getIvory()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getKhaki() {#getKhaki--}
```
public static Color getKhaki()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLavender() {#getLavender--}
```
public static Color getLavender()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLavenderBlush() {#getLavenderBlush--}
```
public static Color getLavenderBlush()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLawnGreen() {#getLawnGreen--}
```
public static Color getLawnGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLemonChiffon() {#getLemonChiffon--}
```
public static Color getLemonChiffon()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightBlue() {#getLightBlue--}
```
public static Color getLightBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightCoral() {#getLightCoral--}
```
public static Color getLightCoral()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightCyan() {#getLightCyan--}
```
public static Color getLightCyan()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightGoldenrodYellow() {#getLightGoldenrodYellow--}
```
public static Color getLightGoldenrodYellow()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightGray() {#getLightGray--}
```
public static Color getLightGray()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightGreen() {#getLightGreen--}
```
public static Color getLightGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightPink() {#getLightPink--}
```
public static Color getLightPink()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSalmon() {#getLightSalmon--}
```
public static Color getLightSalmon()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSeaGreen() {#getLightSeaGreen--}
```
public static Color getLightSeaGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSkyBlue() {#getLightSkyBlue--}
```
public static Color getLightSkyBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSlateGray() {#getLightSlateGray--}
```
public static Color getLightSlateGray()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightSteelBlue() {#getLightSteelBlue--}
```
public static Color getLightSteelBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLightYellow() {#getLightYellow--}
```
public static Color getLightYellow()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLime() {#getLime--}
```
public static Color getLime()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLimeGreen() {#getLimeGreen--}
```
public static Color getLimeGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getLinen() {#getLinen--}
```
public static Color getLinen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMagenta() {#getMagenta--}
```
public static Color getMagenta()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMaroon() {#getMaroon--}
```
public static Color getMaroon()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumAquamarine() {#getMediumAquamarine--}
```
public static Color getMediumAquamarine()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumBlue() {#getMediumBlue--}
```
public static Color getMediumBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumOrchid() {#getMediumOrchid--}
```
public static Color getMediumOrchid()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumPurple() {#getMediumPurple--}
```
public static Color getMediumPurple()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumSeaGreen() {#getMediumSeaGreen--}
```
public static Color getMediumSeaGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumSlateBlue() {#getMediumSlateBlue--}
```
public static Color getMediumSlateBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumSpringGreen() {#getMediumSpringGreen--}
```
public static Color getMediumSpringGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumTurquoise() {#getMediumTurquoise--}
```
public static Color getMediumTurquoise()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMediumVioletRed() {#getMediumVioletRed--}
```
public static Color getMediumVioletRed()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMidnightBlue() {#getMidnightBlue--}
```
public static Color getMidnightBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMintCream() {#getMintCream--}
```
public static Color getMintCream()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMistyRose() {#getMistyRose--}
```
public static Color getMistyRose()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getMoccasin() {#getMoccasin--}
```
public static Color getMoccasin()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getNavajoWhite() {#getNavajoWhite--}
```
public static Color getNavajoWhite()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getNavy() {#getNavy--}
```
public static Color getNavy()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOldLace() {#getOldLace--}
```
public static Color getOldLace()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOlive() {#getOlive--}
```
public static Color getOlive()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOliveDrab() {#getOliveDrab--}
```
public static Color getOliveDrab()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOrange() {#getOrange--}
```
public static Color getOrange()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOrangeRed() {#getOrangeRed--}
```
public static Color getOrangeRed()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getOrchid() {#getOrchid--}
```
public static Color getOrchid()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPaleGoldenrod() {#getPaleGoldenrod--}
```
public static Color getPaleGoldenrod()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPaleGreen() {#getPaleGreen--}
```
public static Color getPaleGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPaleTurquoise() {#getPaleTurquoise--}
```
public static Color getPaleTurquoise()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPaleVioletRed() {#getPaleVioletRed--}
```
public static Color getPaleVioletRed()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPapayaWhip() {#getPapayaWhip--}
```
public static Color getPapayaWhip()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPeachPuff() {#getPeachPuff--}
```
public static Color getPeachPuff()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPeru() {#getPeru--}
```
public static Color getPeru()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPink() {#getPink--}
```
public static Color getPink()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPlum() {#getPlum--}
```
public static Color getPlum()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPowderBlue() {#getPowderBlue--}
```
public static Color getPowderBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getPurple() {#getPurple--}
```
public static Color getPurple()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getR() {#getR--}
```
public byte getR()
```


Получает значение красного компонента этого объекта Color.

**Returns:**
byte — значение красного компонента этого объекта Color.
### getRed() {#getRed--}
```
public static Color getRed()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getRosyBrown() {#getRosyBrown--}
```
public static Color getRosyBrown()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getRoyalBlue() {#getRoyalBlue--}
```
public static Color getRoyalBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSaddleBrown() {#getSaddleBrown--}
```
public static Color getSaddleBrown()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSalmon() {#getSalmon--}
```
public static Color getSalmon()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSandyBrown() {#getSandyBrown--}
```
public static Color getSandyBrown()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSeaGreen() {#getSeaGreen--}
```
public static Color getSeaGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSeaShell() {#getSeaShell--}
```
public static Color getSeaShell()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSienna() {#getSienna--}
```
public static Color getSienna()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSilver() {#getSilver--}
```
public static Color getSilver()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSkyBlue() {#getSkyBlue--}
```
public static Color getSkyBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSlateBlue() {#getSlateBlue--}
```
public static Color getSlateBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSlateGray() {#getSlateGray--}
```
public static Color getSlateGray()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSnow() {#getSnow--}
```
public static Color getSnow()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSpringGreen() {#getSpringGreen--}
```
public static Color getSpringGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getSteelBlue() {#getSteelBlue--}
```
public static Color getSteelBlue()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTan() {#getTan--}
```
public static Color getTan()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTeal() {#getTeal--}
```
public static Color getTeal()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getThistle() {#getThistle--}
```
public static Color getThistle()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTomato() {#getTomato--}
```
public static Color getTomato()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTransparent() {#getTransparent--}
```
public static Color getTransparent()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getTurquoise() {#getTurquoise--}
```
public static Color getTurquoise()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getViolet() {#getViolet--}
```
public static Color getViolet()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getWheat() {#getWheat--}
```
public static Color getWheat()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getWhite() {#getWhite--}
```
public static Color getWhite()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getWhiteSmoke() {#getWhiteSmoke--}
```
public static Color getWhiteSmoke()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getYellow() {#getYellow--}
```
public static Color getYellow()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### getYellowGreen() {#getYellowGreen--}
```
public static Color getYellowGreen()
```


Получить системно‑определённый цвет.

**Returns:**
[Color](../../com.aspose.gridweb/color) - A Color object representing a system-defined color.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Возвращает хеш‑код для этого объекта Color.

**Returns:**
int — целочисленное значение, определяющее хеш‑код этого объекта Color.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Указывает, является ли этот объект Color неинициализированным.

**Returns:**
boolean — это свойство возвращает true, если цвет не инициализирован; иначе false.
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


Получает 32‑битное значение ARGB этого объекта Color.

**Returns:**
int — 32‑битное значение ARGB этого объекта Color.
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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

