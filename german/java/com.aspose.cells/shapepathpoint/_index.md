---
title: "ShapePathPoint"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Geben Sie Positionskoordinaten oder Winkelmarkierungen an."
type: docs
url: /de/java/com.aspose.cells/shapepathpoint/
---

**Inheritance:**
java.lang.Object
```
public class ShapePathPoint
```

Geben Sie Positionskoordinaten oder Winkelmarkierungen an. Positionskoordinaten stellen die Koordinaten eines Pfads in einem Koordinatenraum dar (z. B. X/Y). Winkelmarkierungen zeigen Winkeländerungen in einem Pfad an (z. B. die Start‑ und Schwenkwinkel eines Bogens).
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Gibt den Werttyp des aktuellen Objekts an. |
| [getX()](#getX--) | Liefert die X‑Koordinate für diese Positionskoordinate. |
| [getXAngle()](#getXAngle--) | Wenn das Objekt eine Winkelmarkierung ist, holen oder setzen Sie den ersten Winkel in Grad. |
| [getXPixel()](#getXPixel--) | Wenn das Objekt eine Positionskoordinate ist, holen oder setzen Sie die X‑Koordinate in Pixeln. |
| [getY()](#getY--) | Liefert die Y‑Koordinate für diese Positionskoordinate. |
| [getYAngle()](#getYAngle--) | Wenn das Objekt eine Winkelmarkierung ist, holen oder setzen Sie den zweiten Winkel in Grad. |
| [getYPixel()](#getYPixel--) | Wenn das Objekt eine Positionskoordinate ist, holen oder setzen Sie die Y‑Koordinate in Pixeln. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setX(int value)](#setX-int-) | Setzt die X‑Koordinate für diese Positionskoordinate. |
| [setXAngle(int value)](#setXAngle-int-) | Wenn das Objekt eine Winkelmarkierung ist, holen oder setzen Sie den ersten Winkel in Grad. |
| [setXPixel(int value)](#setXPixel-int-) | Wenn das Objekt eine Positionskoordinate ist, holen oder setzen Sie die X‑Koordinate in Pixeln. |
| [setY(int value)](#setY-int-) | Liefert die Y‑Koordinate für diese Positionskoordinate. |
| [setYAngle(int value)](#setYAngle-int-) | Wenn das Objekt eine Winkelmarkierung ist, holen oder setzen Sie den zweiten Winkel in Grad. |
| [setYPixel(int value)](#setYPixel-int-) | Wenn das Objekt eine Positionskoordinate ist, holen oder setzen Sie die Y‑Koordinate in Pixeln. |
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
### getType() {#getType--}
```
public int getType()
```


Gibt den Werttyp des aktuellen Objekts an.

Siehe [ShapePathPointValueType](../../com.aspose.cells/shapepathpointvaluetype).

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Liefert die X‑Koordinate für diese Positionskoordinate. Einheit EMUs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaften ShapePathPoint.XPixel und ShapePathPoint.XAngle. Diese Eigenschaft wird 12 Monate nach August 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
int
### getXAngle() {#getXAngle--}
```
public int getXAngle()
```


Wenn das Objekt eine Winkelmarkierung ist, holen oder setzen Sie den ersten Winkel in Grad.

**Remarks**

Wenn dieser Winkel der Startwinkel eines Bogens ist. Dieser Winkel gibt an, welcher Winkel entlang des angenommenen Kreiswegs als Startposition zum Zeichnen des Bogens verwendet wird. Dieser Startwinkel wird an die zuletzt bekannte Stiftposition im Shape‑Pfad gesperrt. Dadurch wird ein kontinuierlicher Shape‑Pfad gewährleistet.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Wenn das Objekt eine Positionskoordinate ist, holen oder setzen Sie die X‑Koordinate in Pixeln.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Liest die y‑Koordinate für diese Positionskoordinate. Einheit EMUs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaften ShapePathPoint.YPixel und ShapePathPoint.YAngle. Diese Eigenschaft wird 12 Monate später, seit August 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
int
### getYAngle() {#getYAngle--}
```
public int getYAngle()
```


Wenn das Objekt eine Winkelmarkierung ist, holen oder setzen Sie den zweiten Winkel in Grad.

**Remarks**

Wenn dieser Winkel der Schwenkwinkel eines Bogens ist. Dieser Winkel gibt an, wie weit entlang des angenommenen Kreiswegs der Bogen ausgedehnt wird. Die Erweiterung vom Startwinkel aus erfolgt immer im Uhrzeigersinn um den angenommenen Kreis.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Wenn das Objekt eine Positionskoordinate ist, holen oder setzen Sie die Y‑Koordinate in Pixeln.

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


Setzt die x‑Koordinate für diese Positionskoordinate. Einheit EMUs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaften ShapePathPoint.XPixel und ShapePathPoint.XAngle. Diese Eigenschaft wird 12 Monate nach August 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setXAngle(int value) {#setXAngle-int-}
```
public void setXAngle(int value)
```


Wenn das Objekt eine Winkelmarkierung ist, holen oder setzen Sie den ersten Winkel in Grad.

**Remarks**

Wenn dieser Winkel der Startwinkel eines Bogens ist. Dieser Winkel gibt an, welcher Winkel entlang des angenommenen Kreiswegs als Startposition zum Zeichnen des Bogens verwendet wird. Dieser Startwinkel wird an die zuletzt bekannte Stiftposition im Shape‑Pfad gesperrt. Dadurch wird ein kontinuierlicher Shape‑Pfad gewährleistet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Wenn das Objekt eine Positionskoordinate ist, holen oder setzen Sie die X‑Koordinate in Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Liest die y‑Koordinate für diese Positionskoordinate. Einheit EMUs.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaften ShapePathPoint.YPixel und ShapePathPoint.YAngle. Diese Eigenschaft wird 12 Monate später, seit August 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setYAngle(int value) {#setYAngle-int-}
```
public void setYAngle(int value)
```


Wenn das Objekt eine Winkelmarkierung ist, holen oder setzen Sie den zweiten Winkel in Grad.

**Remarks**

Wenn dieser Winkel der Schwenkwinkel eines Bogens ist. Dieser Winkel gibt an, wie weit entlang des angenommenen Kreiswegs der Bogen ausgedehnt wird. Die Erweiterung vom Startwinkel aus erfolgt immer im Uhrzeigersinn um den angenommenen Kreis.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Wenn das Objekt eine Positionskoordinate ist, holen oder setzen Sie die Y‑Koordinate in Pixeln.

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

