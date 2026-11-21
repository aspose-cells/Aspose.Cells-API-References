---
title: "TextParagraph"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar inställningen för textavsnittet."
type: docs
url: /sv/java/com.aspose.cells/textparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting)
```
public class TextParagraph extends FontSetting
```

Representerar inställningen för textavsnittet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | Hämtar textens horisontella justeringstyp för stycket. |
| [getBullet()](#getBullet--) | Hämtar punkt. |
| [getChildren()](#getChildren--) | Hämtar alla textrader i detta stycke. |
| [getClass()](#getClass--) |  |
| [getDefaultTabSize()](#getDefaultTabSize--) | Hämtar standardstorleken för ett tabulatortecken i detta stycke. |
| [getFirstLineIndent()](#getFirstLineIndent--) | Specificerar indenteringsstorleken som kommer att tillämpas på den första textraden i stycket. |
| [getFont()](#getFont--) | Returnerar teckensnittet för detta objekt. |
| [getFontAlignType()](#getFontAlignType--) | Bestämmer var vertikalt på en textrad de faktiska orden placeras. |
| [getLeftMargin()](#getLeftMargin--) | Specificerar vänstermarginalen för stycket. |
| [getLength()](#getLength--) | Hämtar längden på tecknen. |
| [getLineSpace()](#getLineSpace--) | Hämtar mängden vertikalt blankutrymme som kommer att användas i ett stycke. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--) | Hämtar mängden vertikalt blankutrymme som kommer att användas i ett stycke. |
| [getRightMargin()](#getRightMargin--) | Specificerar högermarginalen för stycket. |
| [getSpaceAfter()](#getSpaceAfter--) | Hämtar mängden vertikala mellanslag som kommer att finnas efter ett stycke. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--) | Hämtar mängden vertikala mellanslag som kommer att finnas efter ett stycke. |
| [getSpaceBefore()](#getSpaceBefore--) | Hämtar mängden vertikala mellanslag som kommer att finnas före ett stycke. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--) | Hämtar mängden vertikala mellanslag som kommer att finnas före ett stycke. |
| [getStartIndex()](#getStartIndex--) | Hämtar startindexet för tecknen. |
| [getStops()](#getStops--) | Hämtar listan med tabbstopp. |
| [getTextOptions()](#getTextOptions--) | Returnerar textalternativen. |
| [getType()](#getType--) | Hämtar typen av textnod. |
| [hashCode()](#hashCode--) |  |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--) | Anger om ett östasiatiskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [isHangingPunctuation()](#isHangingPunctuation--) | Anger om interpunktion ska tvingas placeras på samma rad som texten eller placeras på en annan rad. |
| [isLatinLineBreak()](#isLatinLineBreak--) | Anger om ett latinskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | Ställer in den horisontella justeringstypen för texten i stycket. |
| [setDefaultTabSize(double value)](#setDefaultTabSize-double-) | Ställer in standardstorleken för ett tabulatortecken i detta stycke. |
| [setEastAsianLineBreak(boolean value)](#setEastAsianLineBreak-boolean-) | Anger om ett östasiatiskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [setFirstLineIndent(double value)](#setFirstLineIndent-double-) | Specificerar indenteringsstorleken som kommer att tillämpas på den första textraden i stycket. |
| [setFontAlignType(int value)](#setFontAlignType-int-) | Bestämmer var vertikalt på en textrad de faktiska orden placeras. |
| [setHangingPunctuation(boolean value)](#setHangingPunctuation-boolean-) | Anger om interpunktion ska tvingas placeras på samma rad som texten eller placeras på en annan rad. |
| [setLatinLineBreak(boolean value)](#setLatinLineBreak-boolean-) | Anger om ett latinskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Specificerar vänstermarginalen för stycket. |
| [setLineSpace(double value)](#setLineSpace-double-) | Ställer in mängden vertikala mellanslag som ska användas i ett stycke. |
| [setLineSpaceSizeType(int value)](#setLineSpaceSizeType-int-) | Ställer in mängden vertikala mellanslag som ska användas i ett stycke. |
| [setRightMargin(double value)](#setRightMargin-double-) | Specificerar högermarginalen för stycket. |
| [setSpaceAfter(double value)](#setSpaceAfter-double-) | Ställer in mängden vertikala mellanslag som kommer att finnas efter ett stycke. |
| [setSpaceAfterSizeType(int value)](#setSpaceAfterSizeType-int-) | Ställer in mängden vertikala mellanslag som kommer att finnas efter ett stycke. |
| [setSpaceBefore(double value)](#setSpaceBefore-double-) | Ställer in mängden vertikala mellanslag som kommer att finnas före ett stycke. |
| [setSpaceBeforeSizeType(int value)](#setSpaceBeforeSizeType-int-) | Ställer in mängden vertikala mellanslag som kommer att finnas före ett stycke. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Ställer in den förinställda WordArt-stilen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


Hämtar textens horisontella justeringstyp för stycket.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getBullet() {#getBullet--}
```
public Bullet getBullet()
```


Hämtar punkt.

**Returns:**
[Bullet](../../com.aspose.cells/bullet)
### getChildren() {#getChildren--}
```
public FontSetting[] getChildren()
```


Hämtar alla textkörningar i detta stycke. Om detta stycke är tomt, returnera själva stycket.

**Returns:**
com.aspose.cells.FontSetting[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultTabSize() {#getDefaultTabSize--}
```
public double getDefaultTabSize()
```


Hämtar standardstorleken för ett tabulatortecken i detta stycke.

**Returns:**
double
### getFirstLineIndent() {#getFirstLineIndent--}
```
public double getFirstLineIndent()
```


Specificerar indenteringsstorleken som kommer att tillämpas på den första textraden i stycket.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Returnerar teckensnittet för detta objekt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getFontAlignType() {#getFontAlignType--}
```
public int getFontAlignType()
```


Bestämmer var vertikalt på en textrad de faktiska orden är placerade. Detta handlar om vertikal placering av tecknen i förhållande till baslinjerna.

Se [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Returns:**
int
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Specificerar vänstermarginalen för stycket.

**Returns:**
double
### getLength() {#getLength--}
```
public int getLength()
```


Hämtar längden på tecknen.

**Returns:**
int
### getLineSpace() {#getLineSpace--}
```
public double getLineSpace()
```


Hämtar mängden vertikalt blankutrymme som kommer att användas i ett stycke.

**Returns:**
double
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```
public int getLineSpaceSizeType()
```


Hämtar mängden vertikalt blankutrymme som kommer att användas i ett stycke.

Se [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Specificerar högermarginalen för stycket.

**Returns:**
double
### getSpaceAfter() {#getSpaceAfter--}
```
public double getSpaceAfter()
```


Hämtar mängden vertikala mellanslag som kommer att finnas efter ett stycke.

**Returns:**
double
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```
public int getSpaceAfterSizeType()
```


Hämtar mängden vertikala mellanslag som kommer att finnas efter ett stycke.

Se [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getSpaceBefore() {#getSpaceBefore--}
```
public double getSpaceBefore()
```


Hämtar mängden vertikala mellanslag som kommer att finnas före ett stycke.

**Returns:**
double
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```
public int getSpaceBeforeSizeType()
```


Hämtar mängden vertikala mellanslag som kommer att finnas före ett stycke.

Se [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Hämtar startindexet för tecknen.

**Returns:**
int
### getStops() {#getStops--}
```
public TextTabStopCollection getStops()
```


Hämtar listan med tabbstopp.

**Returns:**
[TextTabStopCollection](../../com.aspose.cells/texttabstopcollection)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Returnerar textalternativen.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Hämtar typen av textnod.

Se [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEastAsianLineBreak() {#isEastAsianLineBreak--}
```
public boolean isEastAsianLineBreak()
```


Anger om ett östasiatiskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till.

**Returns:**
boolean
### isHangingPunctuation() {#isHangingPunctuation--}
```
public boolean isHangingPunctuation()
```


Anger om interpunktion ska tvingas placeras på samma rad som texten eller placeras på en annan rad.

**Returns:**
boolean
### isLatinLineBreak() {#isLatinLineBreak--}
```
public boolean isLatinLineBreak()
```


Anger om ett latinskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till.

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




### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```


Ställer in den horisontella justeringstypen för texten i stycket.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDefaultTabSize(double value) {#setDefaultTabSize-double-}
```
public void setDefaultTabSize(double value)
```


Ställer in standardstorleken för ett tabulatortecken i detta stycke.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setEastAsianLineBreak(boolean value) {#setEastAsianLineBreak-boolean-}
```
public void setEastAsianLineBreak(boolean value)
```


Anger om ett östasiatiskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFirstLineIndent(double value) {#setFirstLineIndent-double-}
```
public void setFirstLineIndent(double value)
```


Specificerar indenteringsstorleken som kommer att tillämpas på den första textraden i stycket.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setFontAlignType(int value) {#setFontAlignType-int-}
```
public void setFontAlignType(int value)
```


Bestämmer var vertikalt på en textrad de faktiska orden är placerade. Detta handlar om vertikal placering av tecknen i förhållande till baslinjerna.

Se [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHangingPunctuation(boolean value) {#setHangingPunctuation-boolean-}
```
public void setHangingPunctuation(boolean value)
```


Anger om interpunktion ska tvingas placeras på samma rad som texten eller placeras på en annan rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLatinLineBreak(boolean value) {#setLatinLineBreak-boolean-}
```
public void setLatinLineBreak(boolean value)
```


Anger om ett latinskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Specificerar vänstermarginalen för stycket.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLineSpace(double value) {#setLineSpace-double-}
```
public void setLineSpace(double value)
```


Ställer in mängden vertikala mellanslag som ska användas i ett stycke.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLineSpaceSizeType(int value) {#setLineSpaceSizeType-int-}
```
public void setLineSpaceSizeType(int value)
```


Ställer in mängden vertikala mellanslag som ska användas i ett stycke.

Se [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Specificerar högermarginalen för stycket.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setSpaceAfter(double value) {#setSpaceAfter-double-}
```
public void setSpaceAfter(double value)
```


Ställer in mängden vertikala mellanslag som kommer att finnas efter ett stycke.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setSpaceAfterSizeType(int value) {#setSpaceAfterSizeType-int-}
```
public void setSpaceAfterSizeType(int value)
```


Ställer in mängden vertikala mellanslag som kommer att finnas efter ett stycke.

Se [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSpaceBefore(double value) {#setSpaceBefore-double-}
```
public void setSpaceBefore(double value)
```


Ställer in mängden vertikala mellanslag som kommer att finnas före ett stycke.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setSpaceBeforeSizeType(int value) {#setSpaceBeforeSizeType-int-}
```
public void setSpaceBeforeSizeType(int value)
```


Ställer in mängden vertikala mellanslag som kommer att finnas före ett stycke.

Se [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Ställer in den förinställda WordArt-stilen.

**Remarks**

Endast för texten i form/diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Den förinställda WordArt-stilen. |

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

