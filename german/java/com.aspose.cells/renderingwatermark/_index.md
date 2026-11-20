---
title: "RenderingWatermark"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Wasserzeichen für die Darstellung."
type: docs
url: /de/java/com.aspose.cells/renderingwatermark/
---

**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```

Wasserzeichen für die Darstellung.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | Erstellt eine Instanz eines Text-Wasserzeichens. |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | Erstellt eine Instanz eines Bild-Wasserzeichens. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Ruft die Schriftart des Wasserzeichens ab. |
| [getHAlignment()](#getHAlignment--) | Ruft die horizontale Ausrichtung des Wasserzeichens zur Seite ab. |
| [getImage()](#getImage--) | Liefert das Bild des Wasserzeichens. |
| [getOffsetX()](#getOffsetX--) | Ermittelt den Offsetwert für [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [getOffsetY()](#getOffsetY--) | Ermittelt den Offsetwert für [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [getOpacity()](#getOpacity--) | Ermittelt die Deckkraft des Wasserzeichens im Bereich [0, 1]. |
| [getRotation()](#getRotation--) | Ermittelt die Drehung des Wasserzeichens in Grad. |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | Ermittelt die Skalierung relativ zur Zielseite in Prozent. |
| [getText()](#getText--) | Ermittelt den Text des Wasserzeichens. |
| [getVAlignment()](#getVAlignment--) | Ermittelt die vertikale Ausrichtung des Wasserzeichens zur Seite. |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | Gibt an, ob das Wasserzeichen hinter dem Seiteninhalt platziert ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | Gibt an, ob das Wasserzeichen hinter dem Seiteninhalt platziert ist. |
| [setHAlignment(int value)](#setHAlignment-int-) | Legt die horizontale Ausrichtung des Wasserzeichens zur Seite fest. |
| [setOffsetX(float value)](#setOffsetX-float-) | Setzt den Offsetwert für [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | Setzt den Offsetwert für [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | Setzt die Deckkraft des Wasserzeichens im Bereich [0, 1]. |
| [setRotation(float value)](#setRotation-float-) | Setzt die Drehung des Wasserzeichens in Grad. |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | Setzt die Skalierung relativ zur Zielseite in Prozent. |
| [setVAlignment(int value)](#setVAlignment-int-) | Setzt die vertikale Ausrichtung des Wasserzeichens zur Seite. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```


Erstellt eine Instanz eines Text-Wasserzeichens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | java.lang.String | Wasserzeichen-Text |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | Wasserzeichen-Schriftart |

### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```


Erstellt eine Instanz eines Bild-Wasserzeichens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageData | byte[] |  |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public RenderingFont getFont()
```


Ruft die Schriftart des Wasserzeichens ab.

**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```


Ruft die horizontale Ausrichtung des Wasserzeichens zur Seite ab.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Nur Links, Mitte, Rechts sind gültig. Standard ist Links.

**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```


Liefert das Bild des Wasserzeichens.

**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```


Ermittelt den Offsetwert für [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```


Ermittelt den Offsetwert für [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```


Ermittelt die Deckkraft des Wasserzeichens im Bereich [0, 1].

**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```


Ermittelt die Drehung des Wasserzeichens in Grad.

**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```


Ermittelt die Skalierung relativ zur Zielseite in Prozent.

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Ermittelt den Text des Wasserzeichens.

**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```


Ermittelt die vertikale Ausrichtung des Wasserzeichens zur Seite.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Nur Oben, Mitte, Unten sind gültig. Standard ist Oben.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBackground() {#isBackground--}
```
public boolean isBackground()
```


Gibt an, ob das Wasserzeichen hinter dem Seiteninhalt platziert ist.

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




### setBackground(boolean value) {#setBackground-boolean-}
```
public void setBackground(boolean value)
```


Gibt an, ob das Wasserzeichen hinter dem Seiteninhalt platziert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```


Legt die horizontale Ausrichtung des Wasserzeichens zur Seite fest.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Nur Links, Mitte, Rechts sind gültig. Standard ist Links.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```


Setzt den Offsetwert für [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```


Setzt den Offsetwert für [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```


Setzt die Deckkraft des Wasserzeichens im Bereich [0, 1].

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```


Setzt die Drehung des Wasserzeichens in Grad.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```


Setzt die Skalierung relativ zur Zielseite in Prozent.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```


Setzt die vertikale Ausrichtung des Wasserzeichens zur Seite.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Nur Oben, Mitte, Unten sind gültig. Standard ist Oben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

