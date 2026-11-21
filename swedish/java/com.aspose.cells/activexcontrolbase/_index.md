---
title: "ActiveXControlBase"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ActiveX‑kontrollen."
type: docs
url: /sv/java/com.aspose.cells/activexcontrolbase/
---

**Inheritance:**
java.lang.Object
```
public abstract class ActiveXControlBase
```

Representerar ActiveX‑kontrollen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Hämtar ole-färgen för bakgrunden. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Hämtar kontrollens binära data. |
| [getForeOleColor()](#getForeOleColor--) | Hämtar förgrundens OLE-färg. |
| [getHeight()](#getHeight--) | Hämtar kontrollens höjd i punktenheter. |
| [getLinkedCell()](#getLinkedCell--) | Hämtar den länkade cellen. |
| [getListFillRange()](#getListFillRange--) | Hämtar listans fyllningsintervall. |
| [getMouseIcon()](#getMouseIcon--) | Hämtar en anpassad ikon som ska visas som muspekare för kontrollen. |
| [getMousePointer()](#getMousePointer--) | Hämtar typen av ikon som visas som muspekare för kontrollen. |
| [getShadow()](#getShadow--) | Indikerar om en skugga ska visas. |
| [getType()](#getType--) | Hämtar typen av ActiveX-kontrollen. |
| [getWidth()](#getWidth--) | Hämtar bredden på kontrollen i enheten punkter. |
| [getWorkbook()](#getWorkbook--) | Hämtar [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) objektet. |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Anger om den här kontrollen är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Ställer in OLE-färgen för bakgrunden. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Ställer in OLE-färgen för förgrunden. |
| [setHeight(double value)](#setHeight-double-) | Ställer in höjden på kontrollen i enheten punkter. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Ställer in den länkade cellen. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Ställer in listfyllningsområdet. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Ställer in en anpassad ikon som ska visas som muspekare för kontrollen. |
| [setMousePointer(int value)](#setMousePointer-int-) | Ställer in typen av ikon som visas som muspekare för kontrollen. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indikerar om en skugga ska visas. |
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




### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Ställer in OLE-färgen för bakgrunden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

