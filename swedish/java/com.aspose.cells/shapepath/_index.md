---
title: "ShapePath"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en skapandeväg bestående av en serie rörelser, linjer och kurvor som när de kombineras bildar en geometrisk form."
type: docs
url: /sv/java/com.aspose.cells/shapepath/
---

**Inheritance:**
java.lang.Object
```
public class ShapePath
```

Representerar en skapelsesökväg bestående av en serie rörelser, linjer och kurvor som när de kombineras bildar en geometrisk form.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [ShapePath()](#ShapePath--) | Initierar en ny instans av klassen [ShapePath](../../com.aspose.cells/shapepath). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | Lägger till en elliptisk båge till den aktuella figuren. |
| [close()](#close--) | Stänger den aktuella figuren och startar en ny figur. |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | Lägger till en kubisk B\u8305zier-kurva till den aktuella figuren. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | Hämtar höjden på denna väg i enheter av pixlar. |
| [getPathSegementList()](#getPathSegementList--) | Hämtar listan [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getPathSegments()](#getPathSegments--) | Hämtar listan [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getWidthPixel()](#getWidthPixel--) | Hämtar bredden på denna väg i enheter av pixlar. |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | Lägger till ett linjesegment till den aktuella figuren. |
| [moveTo(float x, float y)](#moveTo-float-float-) | Startar en ny figur från den angivna punkten utan att stänga den aktuella figuren. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Hämtar höjden på denna väg i enheter av pixlar. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Hämtar bredden på denna väg i enheter av pixlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```


Initierar en ny instans av klassen [ShapePath](../../com.aspose.cells/shapepath).

### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```


Lägger till en elliptisk båge till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| wR | float | Halvbredden på det rektangulära området av \u9225\u5b27\u20ac\u5aa1he-ellipsen som ritar bågen (Enhet: Pixel). |
| hR | float | Halvhöjden på det rektangulära området av \u9225\u5b27\u20ac\u5aa1he-ellipsen som ritar bågen (Enhet: Pixel). |
| stAng | float | Startvinkeln för bågen, mätt i grader medurs från x-axeln (Enhet: Grad). Denna vinkel anger vilken vinkel längs den antagna cirkelbanan som ska användas som startposition för att rita bågen. Denna startvinkel låses till den senast kända pennpositionen i shape path. Detta garanterar en kontinuerlig shape path. |
| swAng | float | Svängvinkeln för en båge. Denna vinkel anger hur långt vinkelnmässigt längs den antagna cirkelbanan bågen kommer att förlängas. Förlängningen från startvinkeln sker alltid i medurs riktning runt den antagna cirkeln. (Enhet: Grad) |

### close() {#close--}
```
public void close()
```


Stänger den aktuella figuren och startar en ny figur. Om den aktuella figuren innehåller en sekvens av sammanhängande linjer och kurvor, stänger metoden loopen genom att ansluta en linje från slutpunkten till startpunkten.

### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```


Lägger till en kubisk B\u8305zier-kurva till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren. Enhet: Pixel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ctrX1 | float | X-koordinaten för den första kontrollpunkten för kurvan (Enhet: Pixel). |
| ctrY1 | float | Y-koordinaten för den första kontrollpunkten för kurvan (Enhet: Pixel). |
| ctrX2 | float | X-koordinaten för den andra kontrollpunkten för kurvan (Enhet: Pixel). |
| ctrY2 | float | Y-koordinaten för den andra kontrollpunkten för kurvan (Enhet: Pixel). |
| endX | float | X-koordinaten för kurvans slutpunkt (Enhet: Pixel). |
| endY | float | Y-koordinaten för kurvans slutpunkt (Enhet: Pixel). |

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
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Hämtar höjden på denna väg i enheter av pixlar.

**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```


Hämtar listan [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället egenskapen ShapePath.PathSegments. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getPathSegments() {#getPathSegments--}
```
public ShapeSegmentPathCollection getPathSegments()
```


Hämtar listan [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Hämtar bredden på denna väg i enheter av pixlar.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### lineTo(float x, float y) {#lineTo-float-float-}
```
public void lineTo(float x, float y)
```


Lägger till ett linjesegment till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren (Enhet: Pixel).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| x | float | X-koordinaten för linjesegmentets slutpunkt (Enhet: Pixel). |
| y | float | Y-koordinaten för linjesegmentets slutpunkt (Enhet: Pixel). |

### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```


Startar en ny figur från den angivna punkten utan att stänga den aktuella figuren. Alla efterföljande punkter som läggs till i banan läggs till i denna nya figur (Enhet: Pixel).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| x | float | X-koordinaten för figurens startpunkt (Enhet: Pixel). |
| y | float | Y-koordinaten för figurens startpunkt (Enhet: Pixel). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Hämtar höjden på denna väg i enheter av pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Hämtar bredden på denna väg i enheter av pixlar.

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

