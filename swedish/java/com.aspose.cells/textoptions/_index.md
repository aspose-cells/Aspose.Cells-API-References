---
title: "TextOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar textalternativen."
type: docs
url: /sv/java/com.aspose.cells/textoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Font](../../com.aspose.cells/font)
```
public class TextOptions extends Font
```

Representerar textalternativen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Kontrollerar om två typsnitt är lika. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Hämtar färgen med ett 32-bitars ARGB-värde. |
| [getCapsType()](#getCapsType--) | Hämtar versaltyp för texter i formen. |
| [getCharset()](#getCharset--) | Representerar teckenuppsättningen. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Hämtar [Color](../../com.aspose.cells/color) för typsnittet. |
| [getDoubleSize()](#getDoubleSize--) | Hämtar dubbel storlek på typsnittet. |
| [getFarEastName()](#getFarEastName--) | Hämtar FarEast-namnet. |
| [getFill()](#getFill--) | Representerar fyllningsformatet för texten. |
| [getKerning()](#getKerning--) | Anger den minsta typsnittsstorleken där teckenkerning sker för detta textsegment. |
| [getLanguageCode()](#getLanguageCode--) | Hämtar språk för användargränssnittet. |
| [getLatinName()](#getLatinName--) | Hämtar latinnamnet. |
| [getName()](#getName--) | Hämtar namnet på formen. |
| [getOutline()](#getOutline--) | Representerar konturformatet för texten. |
| [getSchemeType()](#getSchemeType--) | Hämtar schematypen för typsnittet. |
| [getScriptOffset()](#getScriptOffset--) | Hämtar skriptförskjutningen i procentenheter |
| [getShadow()](#getShadow--) | Representerar ett [ShadowEffect](../../com.aspose.cells/shadoweffect) objekt som specificerar skuggeffekt för diagramelementet eller formen. |
| [getSize()](#getSize--) | Hämtar storleken på typsnittet. |
| [getSpacing()](#getSpacing--) | Anger avståndet mellan tecken inom ett textsegment. |
| [getStrikeType()](#getStrikeType--) | Hämtar genomstrykningstypen för texten. |
| [getThemeColor()](#getThemeColor--) | Hämtar temafärgen. |
| [getUnderline()](#getUnderline--) | Hämtar understrykningsstypen för typsnittet. |
| [getUnderlineColor()](#getUnderlineColor--) | Hämtar färgen på understrykningen. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Hämtar ett värde som indikerar om teckensnittet är fetstil. |
| [isItalic()](#isItalic--) | Hämtar ett värde som indikerar om teckensnittet är kursivt. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Indikerar om normaliseringen av höjden som ska tillämpas på textsekvensen. |
| [isStrikeout()](#isStrikeout--) | Hämtar ett värde som indikerar om teckensnittet har enkel genomstrykning. |
| [isSubscript()](#isSubscript--) | Hämtar ett värde som indikerar om teckensnittet är nedsänkt. |
| [isSuperscript()](#isSuperscript--) | Hämtar ett värde som indikerar om teckensnittet är upphöjt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Ställer in färgen med ett 32-bitars ARGB-värde. |
| [setBold(boolean value)](#setBold-boolean-) | Ställer in ett värde som indikerar om teckensnittet är fetstil. |
| [setCapsType(int value)](#setCapsType-int-) | Ställer in versaltyp för texter i formen. |
| [setCharset(int value)](#setCharset-int-) | Representerar teckenuppsättningen. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Ställer in [Color](../../com.aspose.cells/color) för teckensnittet. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Ställer in dubbel storlek för teckensnittet. |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | Ställer in FarEast-namnet. |
| [setItalic(boolean value)](#setItalic-boolean-) | Ställer in ett värde som indikerar om teckensnittet är kursivt. |
| [setKerning(double value)](#setKerning-double-) | Anger den minsta typsnittsstorleken där teckenkerning sker för detta textsegment. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Ställer in språk för användargränssnittet. |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | Ställer in det latinska namnet. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på formen. |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Ställer in namn och schema för teckensnittet. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indikerar om normaliseringen av höjden som ska tillämpas på textsekvensen. |
| [setSchemeType(int value)](#setSchemeType-int-) | Ställer in schematypen för teckensnittet. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Ställer in skriptförskjutning, i procentenheter |
| [setSize(int value)](#setSize-int-) | Ställer in storleken på teckensnittet. |
| [setSpacing(double value)](#setSpacing-double-) | Anger avståndet mellan tecken inom ett textsegment. |
| [setStrikeType(int value)](#setStrikeType-int-) | Hämtar genomstrykningstypen för texten. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Ställer in ett värde som indikerar om teckensnittet har enkel genomstrykning. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Ställer in ett värde som indikerar om teckensnittet är nedsänkt. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Ställer in ett värde som indikerar om teckensnittet är upphöjt. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Anger temafärgen. |
| [setUnderline(int value)](#setUnderline-int-) | Ställer in teckensnittets understrykningstyp. |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | Ställer in färgen på understrykningen. |
| [toString()](#toString--) | Returnerar en sträng som representerar det aktuella Cell‑objektet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


Kontrollerar om två typsnitt är lika.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | Jämfört teckensnittobjekt. |

**Returns:**
boolesk - Sant om lika med det jämförda teckensnittobjektet.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Hämtar färgen med ett 32-bitars ARGB-värde.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Hämtar versaltyp för texter i formen.

Se [TextCapsType](../../com.aspose.cells/textcapstype).

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


Representerar teckenuppsättningen.

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


Hämtar [Color](../../com.aspose.cells/color) för typsnittet.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Hämtar dubbel storlek på typsnittet.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


Hämtar FarEast-namnet.

**Returns:**
java.lang.String
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Representerar fyllningsformatet för texten.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getKerning() {#getKerning--}
```
public double getKerning()
```


Anger den minsta typsnittsstorleken där teckenkerning sker för detta textsegment.

**Returns:**
double
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Hämtar språk för användargränssnittet.

Se [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


Hämtar latinnamnet.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på formen.

**Returns:**
java.lang.String
### getOutline() {#getOutline--}
```
public LineFormat getOutline()
```


Representerar konturformatet för texten.

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


Hämtar schematypen för typsnittet.

Se [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Hämtar skriptförskjutningen i procentenheter

**Remarks**

Endast för former och diagram.

**Returns:**
double
### getShadow() {#getShadow--}
```
public ShadowEffect getShadow()
```


Representerar ett [ShadowEffect](../../com.aspose.cells/shadoweffect) objekt som specificerar skuggeffekt för diagramelementet eller formen.

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSize() {#getSize--}
```
public int getSize()
```


Hämtar storleken på typsnittet.

**Returns:**
int
### getSpacing() {#getSpacing--}
```
public double getSpacing()
```


Anger avståndet mellan tecken inom ett textsegment.

**Returns:**
double
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


Hämtar genomstrykningstypen för texten.

Se [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Hämtar temafärgen.

**Remarks**

Om teckensnittsfärgen inte är en temafärg returneras NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Hämtar understrykningsstypen för typsnittet.

Se [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


Hämtar färgen på understrykningen.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBold() {#isBold--}
```
public boolean isBold()
```


Hämtar ett värde som indikerar om teckensnittet är fetstil.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Hämtar ett värde som indikerar om teckensnittet är kursivt.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Indikerar om normaliseringen av höjden som ska tillämpas på textsekvensen.

**Remarks**

Endast för teckensnitten i former eller diagram.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


Hämtar ett värde som indikerar om teckensnittet har enkel genomstrykning.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Hämtar ett värde som indikerar om teckensnittet är nedsänkt.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Hämtar ett värde som indikerar om teckensnittet är upphöjt.

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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Ställer in färgen med ett 32-bitars ARGB-värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Ställer in ett värde som indikerar om teckensnittet är fetstil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


Ställer in versaltyp för texter i formen.

Se [TextCapsType](../../com.aspose.cells/textcapstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


Representerar teckenuppsättningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Ställer in [Color](../../com.aspose.cells/color) för teckensnittet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


Ställer in dubbel storlek för teckensnittet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


Ställer in FarEast-namnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Ställer in ett värde som indikerar om teckensnittet är kursivt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


Anger den minsta typsnittsstorleken där teckenkerning sker för detta textsegment.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Ställer in språk för användargränssnittet.

Se [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


Ställer in det latinska namnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


Ställer in namn och schema för teckensnittet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


Indikerar om normaliseringen av höjden som ska tillämpas på textsekvensen.

**Remarks**

Endast för teckensnitten i former eller diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


Ställer in schematypen för teckensnittet.

Se [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


Ställer in skriptförskjutning, i procentenheter

**Remarks**

Endast för former och diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


Ställer in storleken på teckensnittet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


Anger avståndet mellan tecken inom ett textsegment.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


Hämtar genomstrykningstypen för texten.

Se [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


Ställer in ett värde som indikerar om teckensnittet har enkel genomstrykning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


Ställer in ett värde som indikerar om teckensnittet är nedsänkt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


Ställer in ett värde som indikerar om teckensnittet är upphöjt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Anger temafärgen.

**Remarks**

Om teckensnittsfärgen inte är en temafärg returneras NULL.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


Ställer in teckensnittets understrykningstyp.

Se [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


Ställer in färgen på understrykningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar det aktuella Cell‑objektet.

**Returns:**
java.lang.String -
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

