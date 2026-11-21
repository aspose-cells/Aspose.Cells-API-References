---
title: "RenderingWatermark"
second_title: "Aspose.Cells för Java API-referens"
description: "Vattenstämpel för rendering."
type: docs
url: /sv/java/com.aspose.cells/renderingwatermark/
---

**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```

Vattenstämpel för rendering.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | Skapar en instans av textvattenstämpel. |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | Skapar en instans av bildvattenstämpel. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Hämtar teckensnittet för vattenstämpeln. |
| [getHAlignment()](#getHAlignment--) | Hämtar horisontell justering av vattenstämpeln på sidan. |
| [getImage()](#getImage--) | Hämtar bilden av vattenstämpeln. |
| [getOffsetX()](#getOffsetX--) | Hämtar förskjutningsvärde till [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [getOffsetY()](#getOffsetY--) | Hämtar förskjutningsvärde till [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [getOpacity()](#getOpacity--) | Hämtar opaciteten för vattenstämpeln i intervallet [0, 1]. |
| [getRotation()](#getRotation--) | Hämtar rotation av vattenstämpeln i grader. |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | Hämtar skala relativt målsidan i procent. |
| [getText()](#getText--) | Hämtar texten för vattenstämpeln. |
| [getVAlignment()](#getVAlignment--) | Hämtar vertikal justering av vattenstämpeln på sidan. |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | Indikerar om vattenstämpeln är placerad bakom sidinnehållet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | Indikerar om vattenstämpeln är placerad bakom sidinnehållet. |
| [setHAlignment(int value)](#setHAlignment-int-) | Ställer in horisontell justering av vattenstämpeln på sidan. |
| [setOffsetX(float value)](#setOffsetX-float-) | Ställer in förskjutningsvärde till [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | Ställer in förskjutningsvärde till [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | Ställer in opaciteten för vattenstämpeln i intervallet [0, 1]. |
| [setRotation(float value)](#setRotation-float-) | Ställer in rotation av vattenstämpeln i grader. |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | Ställer in skala relativt målsidan i procent. |
| [setVAlignment(int value)](#setVAlignment-int-) | Ställer in vertikal justering av vattenstämpeln på sidan. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```


Skapar en instans av textvattenstämpel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | vattenstämpeltext |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | vattenstämpelfont |

### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```


Skapar en instans av bildvattenstämpel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageData | byte[] |  |

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
### getFont() {#getFont--}
```
public RenderingFont getFont()
```


Hämtar teckensnittet för vattenstämpeln.

**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```


Hämtar horisontell justering av vattenstämpeln på sidan.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Endast Vänster, Centrera, Höger är giltiga. Standard är Vänster.

**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```


Hämtar bilden av vattenstämpeln.

**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```


Hämtar förskjutningsvärde till [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```


Hämtar förskjutningsvärde till [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```


Hämtar opaciteten för vattenstämpeln i intervallet [0, 1].

**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```


Hämtar rotation av vattenstämpeln i grader.

**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```


Hämtar skala relativt målsidan i procent.

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Hämtar texten för vattenstämpeln.

**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```


Hämtar vertikal justering av vattenstämpeln på sidan.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Endast Överst, Centrera, Nederst är giltiga. Standard är Överst.

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


Indikerar om vattenstämpeln är placerad bakom sidinnehållet.

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


Indikerar om vattenstämpeln är placerad bakom sidinnehållet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```


Ställer in horisontell justering av vattenstämpeln på sidan.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Endast Vänster, Centrera, Höger är giltiga. Standard är Vänster.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```


Ställer in förskjutningsvärde till [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```


Ställer in förskjutningsvärde till [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```


Ställer in opaciteten för vattenstämpeln i intervallet [0, 1].

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```


Ställer in rotation av vattenstämpeln i grader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```


Ställer in skala relativt målsidan i procent.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```


Ställer in vertikal justering av vattenstämpeln på sidan.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Endast Överst, Centrera, Nederst är giltiga. Standard är Överst.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

