---
title: "ShapePath"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen Erstellungs-Pfad dar, der aus einer Reihe von Bewegungs‑Linien und Kurven besteht, die zusammen eine geometrische Form bilden."
type: docs
url: /de/java/com.aspose.cells/shapepath/
---

**Inheritance:**
java.lang.Object
```
public class ShapePath
```

Stellt einen Erstellungsweg dar, der aus einer Reihe von Bewegungen, Linien und Kurven besteht, die zusammen eine geometrische Form bilden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ShapePath()](#ShapePath--) | Initialisiert eine neue Instanz der Klasse [ShapePath](../../com.aspose.cells/shapepath). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | Fügt dem aktuellen Pfad einen elliptischen Bogen hinzu. |
| [close()](#close--) | Schließt den aktuellen Pfad und startet einen neuen Pfad. |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | Fügt dem aktuellen Pfad eine kubische B\\u8305zier-Kurve hinzu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | Ermittelt die Höhe dieses Pfades in Pixeln. |
| [getPathSegementList()](#getPathSegementList--) | Ermittelt die Liste von [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getPathSegments()](#getPathSegments--) | Ermittelt die Liste von [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getWidthPixel()](#getWidthPixel--) | Ermittelt die Breite dieses Pfades in Pixeln. |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | Fügt dem aktuellen Pfad ein Liniensegment hinzu. |
| [moveTo(float x, float y)](#moveTo-float-float-) | Startet eine neue Figur vom angegebenen Punkt, ohne die aktuelle Figur zu schließen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Ermittelt die Höhe dieses Pfades in Pixeln. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Ermittelt die Breite dieses Pfades in Pixeln. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```


Initialisiert eine neue Instanz der Klasse [ShapePath](../../com.aspose.cells/shapepath).

### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```


Fügt dem aktuellen Pfad einen elliptischen Bogen hinzu. Der Startpunkt ist der Endpunkt des aktuellen Pfads.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| wR | float | Die halbe Breite des rechteckigen Bereichs der \\u9225\\u5b27\\u20ac\\u5aa1he Ellipse, die den Bogen zeichnet (Einheit: Pixel). |
| hR | float | Die halbe Höhe des rechteckigen Bereichs der \\u9225\\u5b27\\u20ac\\u5aa1he Ellipse, die den Bogen zeichnet (Einheit: Pixel). |
| stAng | float | Der Startwinkel des Bogens, gemessen in Grad im Uhrzeigersinn von der x-Achse (Einheit: Grad). Dieser Winkel gibt an, welcher Winkel entlang des angenommenen Kreiswegs als Startposition für das Zeichnen des Bogens verwendet wird. Dieser Startwinkel wird an die zuletzt bekannte Stiftposition im Formpfad gesperrt, wodurch ein kontinuierlicher Formpfad garantiert wird. |
| swAng | float | Der Schwenkwinkel für einen Bogen. Dieser Winkel gibt an, wie weit entlang des angenommenen Kreiswegs der Bogen ausgedehnt wird. Die Erweiterung vom Startwinkel erfolgt stets im Uhrzeigersinn um den angenommenen Kreis.(Einheit: Grad) |

### close() {#close--}
```
public void close()
```


Schließt die aktuelle Figur und startet eine neue Figur. Wenn die aktuelle Figur eine Sequenz verbundener Linien und Kurven enthält, schließt die Methode die Schleife, indem sie eine Linie vom Endpunkt zum Startpunkt verbindet.

### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```


Fügt dem aktuellen Pfad eine kubische B\\u8305zier-Kurve hinzu. Der Startpunkt ist der Endpunkt des aktuellen Pfads. Einheit: Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ctrX1 | float | Die x-Koordinate des ersten Kontrollpunkts der Kurve (Einheit: Pixel). |
| ctrY1 | float | Die y-Koordinate des ersten Kontrollpunkts der Kurve (Einheit: Pixel). |
| ctrX2 | float | Die x-Koordinate des zweiten Kontrollpunkts der Kurve (Einheit: Pixel). |
| ctrY2 | float | Die y-Koordinate des zweiten Kontrollpunkts der Kurve (Einheit: Pixel). |
| endX | float | Die x-Koordinate des Endpunkts der Kurve (Einheit: Pixel). |
| endY | float | Die y-Koordinate des Endpunkts der Kurve (Einheit: Pixel). |

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
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Ermittelt die Höhe dieses Pfades in Pixeln.

**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```


Ermittelt die Liste von [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft **ShapePath.PathSegments**. Diese Eigenschaft wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getPathSegments() {#getPathSegments--}
```
public ShapeSegmentPathCollection getPathSegments()
```


Ermittelt die Liste von [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Ermittelt die Breite dieses Pfades in Pixeln.

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


Fügt dem aktuellen Pfad ein Liniensegment hinzu. Der Startpunkt ist der Endpunkt des aktuellen Pfads. Einheit: Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| x | float | Die x‑Koordinate des Endpunkts des Liniensegments (Einheit: Pixel). |
| y | float | Die y‑Koordinate des Endpunkts des Liniensegments (Einheit: Pixel). |

### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```


Startet einen neuen Pfad vom angegebenen Punkt, ohne den aktuellen Pfad zu schließen. Alle nachfolgenden Punkte, die dem Pfad hinzugefügt werden, gehören zu diesem neuen Pfad. Einheit: Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| x | float | Die x‑Koordinate des Startpunkts des Pfads (Einheit: Pixel). |
| y | float | Die y‑Koordinate des Startpunkts des Pfads (Einheit: Pixel). |

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


Ermittelt die Höhe dieses Pfades in Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Ermittelt die Breite dieses Pfades in Pixeln.

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

