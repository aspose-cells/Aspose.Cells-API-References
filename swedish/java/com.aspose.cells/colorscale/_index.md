---
title: "ColorScale"
second_title: "Aspose.Cells för Java API-referens"
description: "Beskriver den villkorliga formateringsregeln ColorScale."
type: docs
url: /sv/java/com.aspose.cells/colorscale/
---

**Inheritance:**
java.lang.Object
```
public class ColorScale
```

Beskriv ColorScale-regeln för villkorsstyrd formatering. Denna villkorsstyrda formateringsregel skapar en graderad färgskala på cellerna.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getIs3ColorScale()](#getIs3ColorScale--) | Indikerar huruvida villkorsstyrd formatering är en 3-färgsskala. |
| [getMaxCfvo()](#getMaxCfvo--) | Hämtar detta ColorScale-maxvärdeobjekt. |
| [getMaxColor()](#getMaxColor--) | Hämtar gradientfärgen för det maximala värdet i intervallet. |
| [getMidCfvo()](#getMidCfvo--) | Hämtar detta ColorScale-mittenvärdeobjekt. |
| [getMidColor()](#getMidColor--) | Hämtar gradientfärgen för det mittersta värdet i intervallet. |
| [getMinCfvo()](#getMinCfvo--) | Hämtar detta ColorScale-minvärdeobjekt. |
| [getMinColor()](#getMinColor--) | Hämtar gradientfärgen för det minsta värdet i intervallet. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIs3ColorScale(boolean value)](#setIs3ColorScale-boolean-) | Indikerar huruvida villkorsstyrd formatering är en 3-färgsskala. |
| [setMaxColor(Color value)](#setMaxColor-com.aspose.cells.Color-) | Ställer in gradientfärgen för det maximala värdet i intervallet. |
| [setMidColor(Color value)](#setMidColor-com.aspose.cells.Color-) | Ställer in gradientfärgen för det mittersta värdet i intervallet. |
| [setMinColor(Color value)](#setMinColor-com.aspose.cells.Color-) | Ställer in gradientfärgen för det minsta värdet i intervallet. |
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


Indikerar huruvida villkorsstyrd formatering är en 3-färgsskala.

**Returns:**
boolean
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Hämtar detta ColorScale-maxvärdeobjekt. Kan inte sätta null eller CFValueObject med typen FormatConditionValueType.Min till det.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxColor() {#getMaxColor--}
```
public Color getMaxColor()
```


Hämtar gradientfärgen för det maximala värdet i intervallet.

**Returns:**
[Color](../../com.aspose.cells/color)
### getMidCfvo() {#getMidCfvo--}
```
public ConditionalFormattingValue getMidCfvo()
```


Hämtar detta ColorScale:s mittvärdesobjekt. Det går inte att sätta CFValueObject med typen FormatConditionValueType.Max eller FormatConditionValueType.Min till det.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMidColor() {#getMidColor--}
```
public Color getMidColor()
```


Hämtar gradientfärgen för det mittersta värdet i intervallet.

**Returns:**
[Color](../../com.aspose.cells/color)
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Hämtar detta ColorScale:s minvärdesobjekt. Det går inte att sätta null eller CFValueObject med typen FormatConditionValueType.Max till det.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinColor() {#getMinColor--}
```
public Color getMinColor()
```


Hämtar gradientfärgen för det minsta värdet i intervallet.

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


Indikerar huruvida villkorsstyrd formatering är en 3-färgsskala.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMaxColor(Color value) {#setMaxColor-com.aspose.cells.Color-}
```
public void setMaxColor(Color value)
```


Ställer in gradientfärgen för det maximala värdet i intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setMidColor(Color value) {#setMidColor-com.aspose.cells.Color-}
```
public void setMidColor(Color value)
```


Ställer in gradientfärgen för det mittersta värdet i intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setMinColor(Color value) {#setMinColor-com.aspose.cells.Color-}
```
public void setMinColor(Color value)
```


Ställer in gradientfärgen för det minsta värdet i intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
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

