---
title: "ActiveXControl"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ActiveX‑kontrollen."
type: docs
url: /sv/java/com.aspose.cells/activexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase)
```
public abstract class ActiveXControl extends ActiveXControlBase
```

Representerar ActiveX‑kontrollen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Hämtar ole-färgen för bakgrunden. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Hämtar kontrollens binära data. |
| [getFont()](#getFont--) | Representerar kontrollens teckensnitt. |
| [getForeOleColor()](#getForeOleColor--) | Hämtar förgrundens OLE-färg. |
| [getHeight()](#getHeight--) | Hämtar kontrollens höjd i punktenheter. |
| [getIMEMode()](#getIMEMode--) | Hämtar standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [getLinkedCell()](#getLinkedCell--) | Hämtar den länkade cellen. |
| [getListFillRange()](#getListFillRange--) | Hämtar listans fyllningsintervall. |
| [getMouseIcon()](#getMouseIcon--) | Hämtar en anpassad ikon som ska visas som muspekare för kontrollen. |
| [getMousePointer()](#getMousePointer--) | Hämtar typen av ikon som visas som muspekare för kontrollen. |
| [getShadow()](#getShadow--) | Indikerar om en skugga ska visas. |
| [getTextAlign()](#getTextAlign--) | Representerar hur texten som används av kontrollen ska justeras. |
| [getType()](#getType--) | Hämtar typen av ActiveX-kontrollen. |
| [getWidth()](#getWidth--) | Hämtar bredden på kontrollen i enheten punkter. |
| [getWorkbook()](#getWorkbook--) | Hämtar [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) objektet. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [isEnabled()](#isEnabled--) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [isLocked()](#isLocked--) | Anger om data i kontrollen är låst för redigering. |
| [isTransparent()](#isTransparent--) | Anger om kontrollen är transparent. |
| [isVisible()](#isVisible--) | Anger om den här kontrollen är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Ställer in OLE-färgen för bakgrunden. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Ställer in OLE-färgen för förgrunden. |
| [setHeight(double value)](#setHeight-double-) | Ställer in höjden på kontrollen i enheten punkter. |
| [setIMEMode(int value)](#setIMEMode-int-) | Ställer in standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Ställer in den länkade cellen. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Ställer in listfyllningsområdet. |
| [setLocked(boolean value)](#setLocked-boolean-) | Anger om data i kontrollen är låst för redigering. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Ställer in en anpassad ikon som ska visas som muspekare för kontrollen. |
| [setMousePointer(int value)](#setMousePointer-int-) | Ställer in typen av ikon som visas som muspekare för kontrollen. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indikerar om en skugga ska visas. |
| [setTextAlign(int value)](#setTextAlign-int-) | Representerar hur texten som används av kontrollen ska justeras. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Anger om kontrollen är transparent. |
| [setVisible(boolean value)](#setVisible-boolean-) | Anger om den här kontrollen är synlig. |
| [setWidth(double value)](#setWidth-double-) | Ställer in bredden på kontrollen i enheten punkter. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Hämtar ole-färgen för bakgrunden.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


Hämtar kontrollens binära data.

**Returns:**
byte[]
### getFont() {#getFont--}
```
public Font getFont()
```


Representerar kontrollens teckensnitt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Hämtar förgrundens OLE-färg.

**Remarks**

Gäller inte för bildkontrollen.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Hämtar kontrollens höjd i punktenheter.

**Returns:**
double
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Hämtar standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus.

Se [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Hämtar den länkade cellen.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Hämtar listans fyllningsintervall.

**Returns:**
java.lang.String
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Hämtar en anpassad ikon som ska visas som muspekare för kontrollen.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Hämtar typen av ikon som visas som muspekare för kontrollen.

Se [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indikerar om en skugga ska visas.

**Returns:**
boolean
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Representerar hur texten som används av kontrollen ska justeras.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public abstract int getType()
```


Hämtar typen av ActiveX-kontrollen.

Se [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Hämtar bredden på kontrollen i enheten punkter.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Hämtar [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) objektet.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Anger om data i kontrollen är låst för redigering.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


Anger om kontrollen är transparent.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Anger om den här kontrollen är synlig.

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




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Ställer in OLE-färgen för bakgrunden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Ställer in OLE-färgen för förgrunden.

**Remarks**

Gäller inte för bildkontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Ställer in höjden på kontrollen i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Ställer in standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus.

Se [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Ställer in den länkade cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Ställer in listfyllningsområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Anger om data i kontrollen är låst för redigering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Ställer in en anpassad ikon som ska visas som muspekare för kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Ställer in typen av ikon som visas som muspekare för kontrollen.

Se [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indikerar om en skugga ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Representerar hur texten som används av kontrollen ska justeras.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Anger om kontrollen är transparent.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Anger om den här kontrollen är synlig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Ställer in bredden på kontrollen i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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

