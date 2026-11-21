---
title: "Font"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar typsnittsobjektet som används i ett kalkylblad."
type: docs
url: /sv/java/com.aspose.cells/font/
---

**Inheritance:**
java.lang.Object
```
public class Font
```

Inkapslar typsnittsobjektet som används i ett kalkylblad.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Hello Aspose!");
 
         Font font = cell.getStyle().getFont();
 
         //Setting the font name to "Times New Roman"
         font.setName("Times New Roman");
 
         //Setting font size to 14
         font.setSize(14);
 
         //setting font color as Red
         font.setColor(com.aspose.cells.Color.getRed());           
 
         //Saving the Excel file
         workbook.save("dest.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Kontrollerar om två typsnitt är lika. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Hämtar färgen med ett 32-bitars ARGB-värde. |
| [getCapsType()](#getCapsType--) | Hämtar typ av textversaler. |
| [getCharset()](#getCharset--) | Representerar teckenuppsättningen. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Hämtar [Color](../../com.aspose.cells/color) för typsnittet. |
| [getDoubleSize()](#getDoubleSize--) | Hämtar dubbel storlek på typsnittet. |
| [getName()](#getName--) | Hämtar namnet på [Font](../../com.aspose.cells/font). |
| [getSchemeType()](#getSchemeType--) | Hämtar schematypen för typsnittet. |
| [getScriptOffset()](#getScriptOffset--) | Hämtar skriptförskjutningen i procentenheter |
| [getSize()](#getSize--) | Hämtar storleken på typsnittet. |
| [getStrikeType()](#getStrikeType--) | Hämtar genomstrykningstypen för texten. |
| [getThemeColor()](#getThemeColor--) | Hämtar temafärgen. |
| [getUnderline()](#getUnderline--) | Hämtar understrykningsstypen för typsnittet. |
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
| [setCapsType(int value)](#setCapsType-int-) | Ställer in typ av textversaler. |
| [setCharset(int value)](#setCharset-int-) | Representerar teckenuppsättningen. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Ställer in [Color](../../com.aspose.cells/color) för teckensnittet. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Ställer in dubbel storlek för teckensnittet. |
| [setItalic(boolean value)](#setItalic-boolean-) | Ställer in ett värde som indikerar om teckensnittet är kursivt. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på [Font](../../com.aspose.cells/font). |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Ställer in namn och schema för teckensnittet. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indikerar om normaliseringen av höjden som ska tillämpas på textsekvensen. |
| [setSchemeType(int value)](#setSchemeType-int-) | Ställer in schematypen för teckensnittet. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Ställer in skriptförskjutning, i procentenheter |
| [setSize(int value)](#setSize-int-) | Ställer in storleken på teckensnittet. |
| [setStrikeType(int value)](#setStrikeType-int-) | Hämtar genomstrykningstypen för texten. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Ställer in ett värde som indikerar om teckensnittet har enkel genomstrykning. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Ställer in ett värde som indikerar om teckensnittet är nedsänkt. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Ställer in ett värde som indikerar om teckensnittet är upphöjt. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Anger temafärgen. |
| [setUnderline(int value)](#setUnderline-int-) | Ställer in teckensnittets understrykningstyp. |
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


Hämtar typ av textversaler.

Se [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Endast för teckensnitten i Shapes eller Charts. OBS: Denna medlem är nu föråldrad. Använd istället [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på [Font](../../com.aspose.cells/font).

**Remarks**

Om denna egenskap används för att sätta namnet på teckensnittet, kommer [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) att uppdateras till [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

**Returns:**
java.lang.String
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
### getSize() {#getSize--}
```
public int getSize()
```


Hämtar storleken på typsnittet.

**Returns:**
int
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

Endast för teckensnitten i Shapes eller Charts. OBS: Denna medlem är nu föråldrad. Använd istället [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Ställer in typ av textversaler.

Se [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Endast för teckensnitten i Shapes eller Charts. OBS: Denna medlem är nu föråldrad. Använd istället [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Ställer in ett värde som indikerar om teckensnittet är kursivt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på [Font](../../com.aspose.cells/font).

**Remarks**

Om denna egenskap används för att sätta namnet på teckensnittet, kommer [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) att uppdateras till [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

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

Endast för teckensnitten i Shapes eller Charts. OBS: Denna medlem är nu föråldrad. Använd istället [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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

