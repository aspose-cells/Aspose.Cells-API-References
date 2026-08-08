---
title: "Color"
linktitle: "Color"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents an ARGB (alpha, red, green, blue) color."
type: docs
weight: 640
url: /nodejs/aspose.cells/color/
---

## Color class

Represents an ARGB (alpha, red, green, blue) color.

```js
new Color()
```

construct function

## Methods

| Name | Description |
| --- | --- |
| [equals(obj)](#equals) | Tests whether the specified object is a Color object and is equivalent to this object. |
| [getA()](#geta) | Gets the alpha component value of this Color object. |
| [getB()](#getb) | Gets the blue component value of this Color object. |
| [getG()](#getg) | Gets the green component value of this Color object. |
| [getR()](#getr) | Gets the red component value of this Color object. |
| [hashCode()](#hashcode) | Returns a hash code for this Color object. |
| [isEmpty()](#isempty) | Specifies whether this Color object is uninitialized. |
| [toArgb()](#toargb) | Gets the 32-bit ARGB value of this Color object. |
| [fromArgb(argb)](#fromargb) *(static)* | Creates a Color object from a 32-bit ARGB value. |
| [fromArgb(red, green, blue)](#fromargb-1) *(static)* | Creates a Color object from the specified 8-bit color values (red, green, and blue). The alpha value is implicitly 255 ( |
| [fromArgb(alpha, red, green, blue)](#fromargb-2) *(static)* | Creates a Color object from the four ARGB component (alpha,red, green, and blue) values. Although this method allows a 3 |
| [getAliceBlue()](#getaliceblue) *(static)* | Get a system-defined color. |
| [getAntiqueWhite()](#getantiquewhite) *(static)* | Get a system-defined color. |
| [getAqua()](#getaqua) *(static)* | Get a system-defined color. |
| [getAquamarine()](#getaquamarine) *(static)* | Get a system-defined color. |
| [getAzure()](#getazure) *(static)* | Get a system-defined color. |
| [getBeige()](#getbeige) *(static)* | Get a system-defined color. |
| [getBisque()](#getbisque) *(static)* | Get a system-defined color. |
| [getBlack()](#getblack) *(static)* | Get a system-defined color. |
| [getBlanchedAlmond()](#getblanchedalmond) *(static)* | Get a system-defined color. |
| [getBlue()](#getblue) *(static)* | Get a system-defined color. |
| [getBlueViolet()](#getblueviolet) *(static)* | Get a system-defined color. |
| [getBrown()](#getbrown) *(static)* | Get a system-defined color. |
| [getBurlyWood()](#getburlywood) *(static)* | Get a system-defined color. |
| [getCadetBlue()](#getcadetblue) *(static)* | Get a system-defined color. |
| [getChartreuse()](#getchartreuse) *(static)* | Get a system-defined color. |
| [getChocolate()](#getchocolate) *(static)* | Get a system-defined color. |
| [getCoral()](#getcoral) *(static)* | Get a system-defined color. |
| [getCornflowerBlue()](#getcornflowerblue) *(static)* | Get a system-defined color. |
| [getCornsilk()](#getcornsilk) *(static)* | Get a system-defined color. |
| [getCrimson()](#getcrimson) *(static)* | Get a system-defined color. |
| [getCyan()](#getcyan) *(static)* | Get a system-defined color. |
| [getDarkBlue()](#getdarkblue) *(static)* | Get a system-defined color. |
| [getDarkCyan()](#getdarkcyan) *(static)* | Get a system-defined color. |
| [getDarkGoldenrod()](#getdarkgoldenrod) *(static)* | Get a system-defined color. |
| [getDarkGray()](#getdarkgray) *(static)* | Get a system-defined color. |
| [getDarkGreen()](#getdarkgreen) *(static)* | Get a system-defined color. |
| [getDarkKhaki()](#getdarkkhaki) *(static)* | Get a system-defined color. |
| [getDarkMagenta()](#getdarkmagenta) *(static)* | Get a system-defined color. |
| [getDarkOliveGreen()](#getdarkolivegreen) *(static)* | Get a system-defined color. |
| [getDarkOrange()](#getdarkorange) *(static)* | Get a system-defined color. |
| [getDarkOrchid()](#getdarkorchid) *(static)* | Get a system-defined color. |
| [getDarkRed()](#getdarkred) *(static)* | Get a system-defined color. |
| [getDarkSalmon()](#getdarksalmon) *(static)* | Get a system-defined color. |
| [getDarkSeaGreen()](#getdarkseagreen) *(static)* | Get a system-defined color. |
| [getDarkSlateBlue()](#getdarkslateblue) *(static)* | Get a system-defined color. |
| [getDarkSlateGray()](#getdarkslategray) *(static)* | Get a system-defined color. |
| [getDarkTurquoise()](#getdarkturquoise) *(static)* | Get a system-defined color. |
| [getDarkViolet()](#getdarkviolet) *(static)* | Get a system-defined color. |
| [getDeepPink()](#getdeeppink) *(static)* | Get a system-defined color. |
| [getDeepSkyBlue()](#getdeepskyblue) *(static)* | Get a system-defined color. |
| [getDimGray()](#getdimgray) *(static)* | Get a system-defined color. |
| [getDodgerBlue()](#getdodgerblue) *(static)* | Get a system-defined color. |
| [getEmpty()](#getempty) *(static)* | Get a system-defined empty color. |
| [getFirebrick()](#getfirebrick) *(static)* | Get a system-defined color. |
| [getFloralWhite()](#getfloralwhite) *(static)* | Get a system-defined color. |
| [getForestGreen()](#getforestgreen) *(static)* | Get a system-defined color. |
| [getFuchsia()](#getfuchsia) *(static)* | Get a system-defined color. |
| [getGainsboro()](#getgainsboro) *(static)* | Get a system-defined color. |
| [getGhostWhite()](#getghostwhite) *(static)* | Get a system-defined color. |
| [getGold()](#getgold) *(static)* | Get a system-defined color. |
| [getGoldenrod()](#getgoldenrod) *(static)* | Get a system-defined color. |
| [getGray()](#getgray) *(static)* | Get a system-defined color. |
| [getGreen()](#getgreen) *(static)* | Get a system-defined color. |
| [getGreenYellow()](#getgreenyellow) *(static)* | Get a system-defined color. |
| [getHoneydew()](#gethoneydew) *(static)* | Get a system-defined color. |
| [getHotPink()](#gethotpink) *(static)* | Get a system-defined color. |
| [getIndianRed()](#getindianred) *(static)* | Get a system-defined color. |
| [getIndigo()](#getindigo) *(static)* | Get a system-defined color. |
| [getIvory()](#getivory) *(static)* | Get a system-defined color. |
| [getKhaki()](#getkhaki) *(static)* | Get a system-defined color. |
| [getLavender()](#getlavender) *(static)* | Get a system-defined color. |
| [getLavenderBlush()](#getlavenderblush) *(static)* | Get a system-defined color. |
| [getLawnGreen()](#getlawngreen) *(static)* | Get a system-defined color. |
| [getLemonChiffon()](#getlemonchiffon) *(static)* | Get a system-defined color. |
| [getLightBlue()](#getlightblue) *(static)* | Get a system-defined color. |
| [getLightCoral()](#getlightcoral) *(static)* | Get a system-defined color. |
| [getLightCyan()](#getlightcyan) *(static)* | Get a system-defined color. |
| [getLightGoldenrodYellow()](#getlightgoldenrodyellow) *(static)* | Get a system-defined color. |
| [getLightGray()](#getlightgray) *(static)* | Get a system-defined color. |
| [getLightGreen()](#getlightgreen) *(static)* | Get a system-defined color. |
| [getLightPink()](#getlightpink) *(static)* | Get a system-defined color. |
| [getLightSalmon()](#getlightsalmon) *(static)* | Get a system-defined color. |
| [getLightSeaGreen()](#getlightseagreen) *(static)* | Get a system-defined color. |
| [getLightSkyBlue()](#getlightskyblue) *(static)* | Get a system-defined color. |
| [getLightSlateGray()](#getlightslategray) *(static)* | Get a system-defined color. |
| [getLightSteelBlue()](#getlightsteelblue) *(static)* | Get a system-defined color. |
| [getLightYellow()](#getlightyellow) *(static)* | Get a system-defined color. |
| [getLime()](#getlime) *(static)* | Get a system-defined color. |
| [getLimeGreen()](#getlimegreen) *(static)* | Get a system-defined color. |
| [getLinen()](#getlinen) *(static)* | Get a system-defined color. |
| [getMagenta()](#getmagenta) *(static)* | Get a system-defined color. |
| [getMaroon()](#getmaroon) *(static)* | Get a system-defined color. |
| [getMediumAquamarine()](#getmediumaquamarine) *(static)* | Get a system-defined color. |
| [getMediumBlue()](#getmediumblue) *(static)* | Get a system-defined color. |
| [getMediumOrchid()](#getmediumorchid) *(static)* | Get a system-defined color. |
| [getMediumPurple()](#getmediumpurple) *(static)* | Get a system-defined color. |
| [getMediumSeaGreen()](#getmediumseagreen) *(static)* | Get a system-defined color. |
| [getMediumSlateBlue()](#getmediumslateblue) *(static)* | Get a system-defined color. |
| [getMediumSpringGreen()](#getmediumspringgreen) *(static)* | Get a system-defined color. |
| [getMediumTurquoise()](#getmediumturquoise) *(static)* | Get a system-defined color. |
| [getMediumVioletRed()](#getmediumvioletred) *(static)* | Get a system-defined color. |
| [getMidnightBlue()](#getmidnightblue) *(static)* | Get a system-defined color. |
| [getMintCream()](#getmintcream) *(static)* | Get a system-defined color. |
| [getMistyRose()](#getmistyrose) *(static)* | Get a system-defined color. |
| [getMoccasin()](#getmoccasin) *(static)* | Get a system-defined color. |
| [getNavajoWhite()](#getnavajowhite) *(static)* | Get a system-defined color. |
| [getNavy()](#getnavy) *(static)* | Get a system-defined color. |
| [getOldLace()](#getoldlace) *(static)* | Get a system-defined color. |
| [getOlive()](#getolive) *(static)* | Get a system-defined color. |
| [getOliveDrab()](#getolivedrab) *(static)* | Get a system-defined color. |
| [getOrange()](#getorange) *(static)* | Get a system-defined color. |
| [getOrangeRed()](#getorangered) *(static)* | Get a system-defined color. |
| [getOrchid()](#getorchid) *(static)* | Get a system-defined color. |
| [getPaleGoldenrod()](#getpalegoldenrod) *(static)* | Get a system-defined color. |
| [getPaleGreen()](#getpalegreen) *(static)* | Get a system-defined color. |
| [getPaleTurquoise()](#getpaleturquoise) *(static)* | Get a system-defined color. |
| [getPaleVioletRed()](#getpalevioletred) *(static)* | Get a system-defined color. |
| [getPapayaWhip()](#getpapayawhip) *(static)* | Get a system-defined color. |
| [getPeachPuff()](#getpeachpuff) *(static)* | Get a system-defined color. |
| [getPeru()](#getperu) *(static)* | Get a system-defined color. |
| [getPink()](#getpink) *(static)* | Get a system-defined color. |
| [getPlum()](#getplum) *(static)* | Get a system-defined color. |
| [getPowderBlue()](#getpowderblue) *(static)* | Get a system-defined color. |
| [getPurple()](#getpurple) *(static)* | Get a system-defined color. |
| [getRed()](#getred) *(static)* | Get a system-defined color. |
| [getRosyBrown()](#getrosybrown) *(static)* | Get a system-defined color. |
| [getRoyalBlue()](#getroyalblue) *(static)* | Get a system-defined color. |
| [getSaddleBrown()](#getsaddlebrown) *(static)* | Get a system-defined color. |
| [getSalmon()](#getsalmon) *(static)* | Get a system-defined color. |
| [getSandyBrown()](#getsandybrown) *(static)* | Get a system-defined color. |
| [getSeaGreen()](#getseagreen) *(static)* | Get a system-defined color. |
| [getSeaShell()](#getseashell) *(static)* | Get a system-defined color. |
| [getSienna()](#getsienna) *(static)* | Get a system-defined color. |
| [getSilver()](#getsilver) *(static)* | Get a system-defined color. |
| [getSkyBlue()](#getskyblue) *(static)* | Get a system-defined color. |
| [getSlateBlue()](#getslateblue) *(static)* | Get a system-defined color. |
| [getSlateGray()](#getslategray) *(static)* | Get a system-defined color. |
| [getSnow()](#getsnow) *(static)* | Get a system-defined color. |
| [getSpringGreen()](#getspringgreen) *(static)* | Get a system-defined color. |
| [getSteelBlue()](#getsteelblue) *(static)* | Get a system-defined color. |
| [getTan()](#gettan) *(static)* | Get a system-defined color. |
| [getTeal()](#getteal) *(static)* | Get a system-defined color. |
| [getThistle()](#getthistle) *(static)* | Get a system-defined color. |
| [getTomato()](#gettomato) *(static)* | Get a system-defined color. |
| [getTransparent()](#gettransparent) *(static)* | Get a system-defined color. |
| [getTurquoise()](#getturquoise) *(static)* | Get a system-defined color. |
| [getViolet()](#getviolet) *(static)* | Get a system-defined color. |
| [getWheat()](#getwheat) *(static)* | Get a system-defined color. |
| [getWhite()](#getwhite) *(static)* | Get a system-defined color. |
| [getWhiteSmoke()](#getwhitesmoke) *(static)* | Get a system-defined color. |
| [getYellow()](#getyellow) *(static)* | Get a system-defined color. |
| [getYellowGreen()](#getyellowgreen) *(static)* | Get a system-defined color. |

### equals(obj) {#equals}

Tests whether the specified object is a Color object and is equivalent to this object.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object to test. |

**Returns:** boolean — `boolean` true if obj is a Color object and equivalent to this Color object; otherwise, false.

### getA() {#geta}

Gets the alpha component value of this Color object.

**Returns:** byte — `byte` The alpha component value of this Color object.

### getB() {#getb}

Gets the blue component value of this Color object.

**Returns:** byte — `byte` The blue component value of this Color object.

### getG() {#getg}

Gets the green component value of this Color object.

**Returns:** byte — `byte` The green component value of this Color object.

### getR() {#getr}

Gets the red component value of this Color object.

**Returns:** byte — `byte` The red component value of this Color object.

### hashCode() {#hashcode}

Returns a hash code for this Color object.

**Returns:** Number — `Number` An integer value that specifies the hash code for this Color object.

### isEmpty() {#isempty}

Specifies whether this Color object is uninitialized.

**Returns:** boolean — `boolean` This property returns true if this color is uninitialized; otherwise, false.

### toArgb() {#toargb}

Gets the 32-bit ARGB value of this Color object.

**Returns:** Number — `Number` The 32-bit ARGB value of this Color object.

### fromArgb(argb) (static) {#fromargb}

Creates a Color object from a 32-bit ARGB value.

| Parameter | Type | Description |
| --- | --- | --- |
| argb | Number | A value specifying the 32-bit ARGB value. |

**Returns:** Color — `Color` The Color object that this method creates.

### fromArgb(red, green, blue) (static) {#fromargb-1}

Creates a Color object from the specified 8-bit color values (red, green, and blue). The alpha value is implicitly 255 (fully opaque). Although this method allows a 32-bit value to be passed for each color component, the value of each component is limited to 8 bits.

| Parameter | Type | Description |
| --- | --- | --- |
| red | Number | The red component value for the new Color object. Valid values are 0 through 255. |
| green | Number | The green component value for the new Color object. Valid values are 0 through 255. |
| blue | Number | The blue component value for the new Color object. Valid values are 0 through 255. |

**Returns:** Color — `Color` The Color object that this method creates.

### fromArgb(alpha, red, green, blue) (static) {#fromargb-2}

Creates a Color object from the four ARGB component (alpha,red, green, and blue) values. Although this method allows a 32-bit value to be passed for each component, the value of each component is limited to 8 bits.

| Parameter | Type | Description |
| --- | --- | --- |
| alpha | Number | The alpha component. Valid values are 0 through 255. |
| red | Number | The red component. Valid values are 0 through 255. |
| green | Number | The green component. Valid values are 0 through 255. |
| blue | Number | The blue component. Valid values are 0 through 255. |

**Returns:** Color — `Color` The Color object that this method creates.

### getAliceBlue() (static) {#getaliceblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getAntiqueWhite() (static) {#getantiquewhite}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getAqua() (static) {#getaqua}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getAquamarine() (static) {#getaquamarine}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getAzure() (static) {#getazure}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getBeige() (static) {#getbeige}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getBisque() (static) {#getbisque}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getBlack() (static) {#getblack}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getBlanchedAlmond() (static) {#getblanchedalmond}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getBlue() (static) {#getblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getBlueViolet() (static) {#getblueviolet}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getBrown() (static) {#getbrown}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getBurlyWood() (static) {#getburlywood}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getCadetBlue() (static) {#getcadetblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getChartreuse() (static) {#getchartreuse}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getChocolate() (static) {#getchocolate}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getCoral() (static) {#getcoral}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getCornflowerBlue() (static) {#getcornflowerblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getCornsilk() (static) {#getcornsilk}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getCrimson() (static) {#getcrimson}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getCyan() (static) {#getcyan}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkBlue() (static) {#getdarkblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkCyan() (static) {#getdarkcyan}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkGoldenrod() (static) {#getdarkgoldenrod}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkGray() (static) {#getdarkgray}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkGreen() (static) {#getdarkgreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkKhaki() (static) {#getdarkkhaki}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkMagenta() (static) {#getdarkmagenta}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkOliveGreen() (static) {#getdarkolivegreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkOrange() (static) {#getdarkorange}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkOrchid() (static) {#getdarkorchid}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkRed() (static) {#getdarkred}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkSalmon() (static) {#getdarksalmon}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkSeaGreen() (static) {#getdarkseagreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkSlateBlue() (static) {#getdarkslateblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkSlateGray() (static) {#getdarkslategray}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkTurquoise() (static) {#getdarkturquoise}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDarkViolet() (static) {#getdarkviolet}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDeepPink() (static) {#getdeeppink}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDeepSkyBlue() (static) {#getdeepskyblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDimGray() (static) {#getdimgray}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getDodgerBlue() (static) {#getdodgerblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getEmpty() (static) {#getempty}

Get a system-defined empty color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getFirebrick() (static) {#getfirebrick}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getFloralWhite() (static) {#getfloralwhite}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getForestGreen() (static) {#getforestgreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getFuchsia() (static) {#getfuchsia}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getGainsboro() (static) {#getgainsboro}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getGhostWhite() (static) {#getghostwhite}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getGold() (static) {#getgold}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getGoldenrod() (static) {#getgoldenrod}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getGray() (static) {#getgray}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getGreen() (static) {#getgreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getGreenYellow() (static) {#getgreenyellow}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getHoneydew() (static) {#gethoneydew}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getHotPink() (static) {#gethotpink}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getIndianRed() (static) {#getindianred}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getIndigo() (static) {#getindigo}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getIvory() (static) {#getivory}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getKhaki() (static) {#getkhaki}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLavender() (static) {#getlavender}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLavenderBlush() (static) {#getlavenderblush}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLawnGreen() (static) {#getlawngreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLemonChiffon() (static) {#getlemonchiffon}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightBlue() (static) {#getlightblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightCoral() (static) {#getlightcoral}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightCyan() (static) {#getlightcyan}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightGoldenrodYellow() (static) {#getlightgoldenrodyellow}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightGray() (static) {#getlightgray}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightGreen() (static) {#getlightgreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightPink() (static) {#getlightpink}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightSalmon() (static) {#getlightsalmon}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightSeaGreen() (static) {#getlightseagreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightSkyBlue() (static) {#getlightskyblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightSlateGray() (static) {#getlightslategray}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightSteelBlue() (static) {#getlightsteelblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLightYellow() (static) {#getlightyellow}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLime() (static) {#getlime}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLimeGreen() (static) {#getlimegreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getLinen() (static) {#getlinen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMagenta() (static) {#getmagenta}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMaroon() (static) {#getmaroon}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMediumAquamarine() (static) {#getmediumaquamarine}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMediumBlue() (static) {#getmediumblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMediumOrchid() (static) {#getmediumorchid}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMediumPurple() (static) {#getmediumpurple}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMediumSeaGreen() (static) {#getmediumseagreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMediumSlateBlue() (static) {#getmediumslateblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMediumSpringGreen() (static) {#getmediumspringgreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMediumTurquoise() (static) {#getmediumturquoise}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMediumVioletRed() (static) {#getmediumvioletred}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMidnightBlue() (static) {#getmidnightblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMintCream() (static) {#getmintcream}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMistyRose() (static) {#getmistyrose}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getMoccasin() (static) {#getmoccasin}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getNavajoWhite() (static) {#getnavajowhite}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getNavy() (static) {#getnavy}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getOldLace() (static) {#getoldlace}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getOlive() (static) {#getolive}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getOliveDrab() (static) {#getolivedrab}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getOrange() (static) {#getorange}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getOrangeRed() (static) {#getorangered}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getOrchid() (static) {#getorchid}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPaleGoldenrod() (static) {#getpalegoldenrod}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPaleGreen() (static) {#getpalegreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPaleTurquoise() (static) {#getpaleturquoise}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPaleVioletRed() (static) {#getpalevioletred}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPapayaWhip() (static) {#getpapayawhip}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPeachPuff() (static) {#getpeachpuff}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPeru() (static) {#getperu}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPink() (static) {#getpink}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPlum() (static) {#getplum}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPowderBlue() (static) {#getpowderblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getPurple() (static) {#getpurple}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getRed() (static) {#getred}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getRosyBrown() (static) {#getrosybrown}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getRoyalBlue() (static) {#getroyalblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSaddleBrown() (static) {#getsaddlebrown}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSalmon() (static) {#getsalmon}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSandyBrown() (static) {#getsandybrown}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSeaGreen() (static) {#getseagreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSeaShell() (static) {#getseashell}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSienna() (static) {#getsienna}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSilver() (static) {#getsilver}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSkyBlue() (static) {#getskyblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSlateBlue() (static) {#getslateblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSlateGray() (static) {#getslategray}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSnow() (static) {#getsnow}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSpringGreen() (static) {#getspringgreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getSteelBlue() (static) {#getsteelblue}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getTan() (static) {#gettan}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getTeal() (static) {#getteal}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getThistle() (static) {#getthistle}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getTomato() (static) {#gettomato}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getTransparent() (static) {#gettransparent}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getTurquoise() (static) {#getturquoise}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getViolet() (static) {#getviolet}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getWheat() (static) {#getwheat}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getWhite() (static) {#getwhite}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getWhiteSmoke() (static) {#getwhitesmoke}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getYellow() (static) {#getyellow}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.

### getYellowGreen() (static) {#getyellowgreen}

Get a system-defined color.

**Returns:** Color — `Color` A Color object representing a system-defined color.
