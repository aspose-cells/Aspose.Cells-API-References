---
title: "MsoFillFormat"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Füllformatierung für eine Form dar."
type: docs
url: /de/java/com.aspose.cells/msofillformat/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormat
```

Stellt die Füllformatierung für eine Form dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Liest die Hintergrundfarbe der Datei. |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | Liest die Vordergrundfarbe der Füllung. |
| [getImageData()](#getImageData--) | Liest die Textur- und Bildfüllungsdaten. |
| [getTexture()](#getTexture--) | Liest den Texturfülltyp. |
| [getTransparency()](#getTransparency--) | Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Gibt an, ob eine Füllung vorhanden ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | Setzt die Hintergrundfarbe der Datei. |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | Setzt die Vordergrundfarbe der Füllung. |
| [setImageData(byte[] value)](#setImageData-byte---) | Setzt die Textur- und Bildfüllungsdaten. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Setzt die angegebene Füllung auf einen einfarbigen Farbverlauf. |
| [setTransparency(double value)](#setTransparency-double-) | Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [setVisible(boolean value)](#setVisible-boolean-) | Gibt an, ob eine Füllung vorhanden ist. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Liest die Hintergrundfarbe der Datei.

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


Liest die Vordergrundfarbe der Füllung.

**Returns:**
[Color](../../com.aspose.cells/color)
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Liest die Textur- und Bildfüllungsdaten.

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


Liest den Texturfülltyp.

Siehe [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

**Returns:**
double
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


Gibt an, ob eine Füllung vorhanden ist.

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


Setzt die Hintergrundfarbe der Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


Setzt die Vordergrundfarbe der Füllung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Setzt die Textur- und Bildfüllungsdaten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Setzt die angegebene Füllung auf einen einfarbigen Farbverlauf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Eine Farbverlauffarbe. |
| Grad | double | Der Grad des Farbverlaufs. Kann ein Wert von 0.0 (dunkel) bis 1.0 (hell) sein. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Gibt an, ob eine Füllung vorhanden ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

