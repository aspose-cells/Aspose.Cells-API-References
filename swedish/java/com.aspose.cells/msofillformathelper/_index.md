---
title: "MsoFillFormatHelper"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar fyllningsformatering för en figur."
type: docs
url: /sv/java/com.aspose.cells/msofillformathelper/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormatHelper
```

Representerar fyllningsformatering för en figur.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Hämtar filens bakgrundsfärg. |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | Hämtar fyllningens förgrundsfärg. |
| [getForeColorTransparency()](#getForeColorTransparency--) | Returnerar eller anger graden av förgrundsfärg för den angivna fyllningen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [getImageData()](#getImageData--) | Hämtar fyllningsdata för textur och bild. |
| [getTexture()](#getTexture--) | Hämtar typ av texturfyllning. |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Indikerar om det finns fyllning. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | Anger filens bakgrundsfärg. |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | Anger fyllningens förgrundsfärg. |
| [setForeColorTransparency(double value)](#setForeColorTransparency-double-) | Returnerar eller anger graden av förgrundsfärg för den angivna fyllningen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [setImageData(byte[] value)](#setImageData-byte---) | Anger fyllningsdata för textur och bild. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Anger den angivna fyllningen till en enfärgsgradient. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indikerar om det finns fyllning. |
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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Hämtar filens bakgrundsfärg.

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


Hämtar fyllningens förgrundsfärg.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForeColorTransparency() {#getForeColorTransparency--}
```
public double getForeColorTransparency()
```


Returnerar eller anger graden av förgrundsfärg för den angivna fyllningen som ett värde från 0.0 (opak) till 1.0 (klar).

**Returns:**
double
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Hämtar fyllningsdata för textur och bild.

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


Hämtar typ av texturfyllning.

Se [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
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


Indikerar om det finns fyllning.

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


Anger filens bakgrundsfärg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


Anger fyllningens förgrundsfärg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColorTransparency(double value) {#setForeColorTransparency-double-}
```
public void setForeColorTransparency(double value)
```


Returnerar eller anger graden av förgrundsfärg för den angivna fyllningen som ett värde från 0.0 (opak) till 1.0 (klar).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Anger fyllningsdata för textur och bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Anger den angivna fyllningen till en enfärgsgradient.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | En gradientfärg. |
| grad | double | Gradientgraden. Kan vara ett värde från 0.0 (mörk) till 1.0 (ljus). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indikerar om det finns fyllning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

