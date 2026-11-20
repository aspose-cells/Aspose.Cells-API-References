---
title: "ColorScale"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Beschreibt die ColorScale-Bedingte-Formatierungsregel."
type: docs
url: /de/java/com.aspose.cells/colorscale/
---

**Inheritance:**
java.lang.Object
```
public class ColorScale
```

Beschreibt die ColorScale bedingte Formatierungsregel. Diese bedingte Formatierungsregel erstellt eine abgestufte Farbskala in den Zellen.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getIs3ColorScale()](#getIs3ColorScale--) | Gibt an, ob die bedingte Formatierung eine 3‑Farbskala ist. |
| [getMaxCfvo()](#getMaxCfvo--) | Ruft das Maximalwertobjekt dieser ColorScale ab. |
| [getMaxColor()](#getMaxColor--) | Ruft die Farbverlauffarbe für den Maximalwert im Bereich ab. |
| [getMidCfvo()](#getMidCfvo--) | Ruft das Mittelwertobjekt dieser ColorScale ab. |
| [getMidColor()](#getMidColor--) | Ruft die Farbverlauffarbe für den Mittelwert im Bereich ab. |
| [getMinCfvo()](#getMinCfvo--) | Ruft das Minimalwertobjekt dieser ColorScale ab. |
| [getMinColor()](#getMinColor--) | Ruft die Farbverlauffarbe für den Minimalwert im Bereich ab. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIs3ColorScale(boolean value)](#setIs3ColorScale-boolean-) | Gibt an, ob die bedingte Formatierung eine 3‑Farbskala ist. |
| [setMaxColor(Color value)](#setMaxColor-com.aspose.cells.Color-) | Setzt die Farbverlauffarbe für den Maximalwert im Bereich. |
| [setMidColor(Color value)](#setMidColor-com.aspose.cells.Color-) | Setzt die Farbverlauffarbe für den Mittelwert im Bereich. |
| [setMinColor(Color value)](#setMinColor-com.aspose.cells.Color-) | Setzt die Farbverlauffarbe für den Minimalwert im Bereich. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getIs3ColorScale() {#getIs3ColorScale--}
```
public boolean getIs3ColorScale()
```


Gibt an, ob die bedingte Formatierung eine 3‑Farbskala ist.

**Returns:**
boolean
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Ruft das Maximalwertobjekt dieser ColorScale ab. Null oder ein CFValueObject vom Typ FormatConditionValueType.Min kann nicht gesetzt werden.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxColor() {#getMaxColor--}
```
public Color getMaxColor()
```


Ruft die Farbverlauffarbe für den Maximalwert im Bereich ab.

**Returns:**
[Color](../../com.aspose.cells/color)
### getMidCfvo() {#getMidCfvo--}
```
public ConditionalFormattingValue getMidCfvo()
```


Ruft das Mittelwertobjekt dieser ColorScale ab. Ein CFValueObject vom Typ FormatConditionValueType.Max oder FormatConditionValueType.Min kann nicht gesetzt werden.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMidColor() {#getMidColor--}
```
public Color getMidColor()
```


Ruft die Farbverlauffarbe für den Mittelwert im Bereich ab.

**Returns:**
[Color](../../com.aspose.cells/color)
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Ruft das Minimalwertobjekt dieser ColorScale ab. Es kann nicht null oder ein CFValueObject vom Typ FormatConditionValueType.Max zugewiesen werden.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinColor() {#getMinColor--}
```
public Color getMinColor()
```


Ruft die Farbverlauffarbe für den Minimalwert im Bereich ab.

**Returns:**
[Color](../../com.aspose.cells/color)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setIs3ColorScale(boolean value) {#setIs3ColorScale-boolean-}
```
public void setIs3ColorScale(boolean value)
```


Gibt an, ob die bedingte Formatierung eine 3‑Farbskala ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMaxColor(Color value) {#setMaxColor-com.aspose.cells.Color-}
```
public void setMaxColor(Color value)
```


Setzt die Farbverlauffarbe für den Maximalwert im Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setMidColor(Color value) {#setMidColor-com.aspose.cells.Color-}
```
public void setMidColor(Color value)
```


Setzt die Farbverlauffarbe für den Mittelwert im Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setMinColor(Color value) {#setMinColor-com.aspose.cells.Color-}
```
public void setMinColor(Color value)
```


Setzt die Farbverlauffarbe für den Minimalwert im Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

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

