---
title: "ShapePathPoint"
second_title: "Aspose.Cells för Java API-referens"
description: "Ange positionskoordinater eller vinkelmarkörer."
type: docs
url: /sv/java/com.aspose.cells/shapepathpoint/
---

**Inheritance:**
java.lang.Object
```
public class ShapePathPoint
```

Ange positionskoordinater eller vinkelmarkörer. Positionskoordinater representerar koordinaterna för en bana i ett koordinatrum (t.ex. X/Y). Vinkelmarkörer indikerar vinkeländringar i en bana (t.ex. start‑ och svängvinklarna för en båge).
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Anger värdetypen för det aktuella objektet. |
| [getX()](#getX--) | Hämtar x‑koordinaten för denna positionskoordinat. |
| [getXAngle()](#getXAngle--) | När objektet är en vinkelmarkör, hämta eller ange den första vinkeln i grader. |
| [getXPixel()](#getXPixel--) | När objektet är en positionskoordinat, hämta eller ange x‑koordinaten i pixlar. |
| [getY()](#getY--) | Hämtar y‑koordinaten för denna positionskoordinat. |
| [getYAngle()](#getYAngle--) | När objektet är en vinkelmarkör, hämta eller ange den andra vinkeln i grader. |
| [getYPixel()](#getYPixel--) | När objektet är en positionskoordinat, hämta eller ange y‑koordinaten i pixlar. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setX(int value)](#setX-int-) | Ställer in x‑koordinaten för denna positionskoordinat. |
| [setXAngle(int value)](#setXAngle-int-) | När objektet är en vinkelmarkör, hämta eller ange den första vinkeln i grader. |
| [setXPixel(int value)](#setXPixel-int-) | När objektet är en positionskoordinat, hämta eller ange x‑koordinaten i pixlar. |
| [setY(int value)](#setY-int-) | Hämtar y‑koordinaten för denna positionskoordinat. |
| [setYAngle(int value)](#setYAngle-int-) | När objektet är en vinkelmarkör, hämta eller ange den andra vinkeln i grader. |
| [setYPixel(int value)](#setYPixel-int-) | När objektet är en positionskoordinat, hämta eller ange y‑koordinaten i pixlar. |
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
### getType() {#getType--}
```
public int getType()
```


Anger värdetypen för det aktuella objektet.

Se [ShapePathPointValueType](../../com.aspose.cells/shapepathpointvaluetype).

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Hämtar x‑koordinaten för denna positionskoordinat. Enhet EMU.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskaperna ShapePathPoint.XPixel och ShapePathPoint.XAngle. Denna egenskap kommer att tas bort 12 månader senare, från och med augusti 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getXAngle() {#getXAngle--}
```
public int getXAngle()
```


När objektet är en vinkelmarkör, hämta eller ange den första vinkeln i grader.

**Remarks**

Om denna vinkel är startvinkeln för en båge. Denna vinkel anger vilken vinkel längs den antagna cirkelbanan som ska användas som startposition för att rita bågen. Denna startvinkel låses till den senast kända pennpositionen i shape‑banan. Detta garanterar en kontinuerlig shape‑bana.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


När objektet är en positionskoordinat, hämta eller ange x‑koordinaten i pixlar.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Hämtar y‑koordinaten för denna positionskoordinat. Enhet EMU.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället ShapePathPoint.YPixel och ShapePathPoint.YAngle egenskaper. Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getYAngle() {#getYAngle--}
```
public int getYAngle()
```


När objektet är en vinkelmarkör, hämta eller ange den andra vinkeln i grader.

**Remarks**

Om denna vinkel är svängvinkeln för en båge. Denna vinkel kommer att ange hur långt vinkelmässigt längs den påstådda cirkelbanan bågen kommer att förlängas. Förlängningen från startvinkeln kommer alltid att vara i medurs riktning runt den påstådda cirkeln.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


När objektet är en positionskoordinat, hämta eller ange y‑koordinaten i pixlar.

**Returns:**
int
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




### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Ställer in x-koordinaten för denna positionskoordinat. Enhet EMU.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskaperna ShapePathPoint.XPixel och ShapePathPoint.XAngle. Denna egenskap kommer att tas bort 12 månader senare, från och med augusti 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setXAngle(int value) {#setXAngle-int-}
```
public void setXAngle(int value)
```


När objektet är en vinkelmarkör, hämta eller ange den första vinkeln i grader.

**Remarks**

Om denna vinkel är startvinkeln för en båge. Denna vinkel anger vilken vinkel längs den antagna cirkelbanan som ska användas som startposition för att rita bågen. Denna startvinkel låses till den senast kända pennpositionen i shape‑banan. Detta garanterar en kontinuerlig shape‑bana.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


När objektet är en positionskoordinat, hämta eller ange x‑koordinaten i pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Hämtar y‑koordinaten för denna positionskoordinat. Enhet EMU.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället ShapePathPoint.YPixel och ShapePathPoint.YAngle egenskaper. Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setYAngle(int value) {#setYAngle-int-}
```
public void setYAngle(int value)
```


När objektet är en vinkelmarkör, hämta eller ange den andra vinkeln i grader.

**Remarks**

Om denna vinkel är svängvinkeln för en båge. Denna vinkel kommer att ange hur långt vinkelmässigt längs den påstådda cirkelbanan bågen kommer att förlängas. Förlängningen från startvinkeln kommer alltid att vara i medurs riktning runt den påstådda cirkeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


När objektet är en positionskoordinat, hämta eller ange y‑koordinaten i pixlar.

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

