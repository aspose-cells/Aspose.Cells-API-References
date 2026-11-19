---
title: "ShapePathPoint"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifiez les coordonnées de position ou les repères d'angle."
type: docs
url: /fr/java/com.aspose.cells/shapepathpoint/
---

**Inheritance:**
java.lang.Object
```
public class ShapePathPoint
```

Spécifiez les coordonnées de position ou les marqueurs d'angle. Les coordonnées de position représentent les coordonnées d'un chemin dans un espace de coordonnées (e.g. X/Y). Les marqueurs d'angle indiquent les changements angulaires d'un chemin (e.g. les angles de départ et d'arc d'un arc).
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Spécifie le type de valeur de l'objet actuel. |
| [getX()](#getX--) | Obtient la coordonnée x pour cette coordonnée de position. |
| [getXAngle()](#getXAngle--) | Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le premier angle en degrés. |
| [getXPixel()](#getXPixel--) | Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée x en pixels. |
| [getY()](#getY--) | Obtient la coordonnée y pour cette coordonnée de position. |
| [getYAngle()](#getYAngle--) | Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le deuxième angle en degrés. |
| [getYPixel()](#getYPixel--) | Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée y en pixels. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setX(int value)](#setX-int-) | Définit la coordonnée x pour cette coordonnée de position. |
| [setXAngle(int value)](#setXAngle-int-) | Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le premier angle en degrés. |
| [setXPixel(int value)](#setXPixel-int-) | Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée x en pixels. |
| [setY(int value)](#setY-int-) | Obtient la coordonnée y pour cette coordonnée de position. |
| [setYAngle(int value)](#setYAngle-int-) | Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le deuxième angle en degrés. |
| [setYPixel(int value)](#setYPixel-int-) | Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée y en pixels. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
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


Spécifie le type de valeur de l'objet actuel.

Voir [ShapePathPointValueType](../../com.aspose.cells/shapepathpointvaluetype).

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Obtient la coordonnée x pour cette coordonnée de position. Unité EMUs.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser les propriétés ShapePathPoint.XPixel et ShapePathPoint.XAngle. Cette propriété sera supprimée 12 mois plus tard, à compter d’août 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getXAngle() {#getXAngle--}
```
public int getXAngle()
```


Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le premier angle en degrés.

**Remarks**

Si cet angle est l’angle de départ d’un arc. Cet angle spécifiera quel angle le long du chemin circulaire supposé sera utilisé comme position de départ pour tracer l’arc. Cet angle de départ sera verrouillé à la dernière position connue du stylo dans le chemin de forme. Garantissant ainsi un chemin de forme continu.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée x en pixels.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Obtient la coordonnée y pour cette position. Unité : EMU.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser les propriétés ShapePathPoint.YPixel et ShapePathPoint.YAngle. Cette propriété sera supprimée 12 mois plus tard, à compter d’août 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getYAngle() {#getYAngle--}
```
public int getYAngle()
```


Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le deuxième angle en degrés.

**Remarks**

Si cet angle est l’angle d’oscillation d’un arc. Cet angle spécifiera jusqu’où, en termes d’angle, le long du chemin circulaire supposé l’arc sera prolongé. L’extension à partir de l’angle de départ sera toujours dans le sens horaire autour du cercle supposé.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée y en pixels.

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


Définit la coordonnée x pour cette position. Unité : EMU.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser les propriétés ShapePathPoint.XPixel et ShapePathPoint.XAngle. Cette propriété sera supprimée 12 mois plus tard, à compter d’août 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setXAngle(int value) {#setXAngle-int-}
```
public void setXAngle(int value)
```


Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le premier angle en degrés.

**Remarks**

Si cet angle est l’angle de départ d’un arc. Cet angle spécifiera quel angle le long du chemin circulaire supposé sera utilisé comme position de départ pour tracer l’arc. Cet angle de départ sera verrouillé à la dernière position connue du stylo dans le chemin de forme. Garantissant ainsi un chemin de forme continu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée x en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Obtient la coordonnée y pour cette position. Unité : EMU.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser les propriétés ShapePathPoint.YPixel et ShapePathPoint.YAngle. Cette propriété sera supprimée 12 mois plus tard, à compter d’août 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setYAngle(int value) {#setYAngle-int-}
```
public void setYAngle(int value)
```


Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le deuxième angle en degrés.

**Remarks**

Si cet angle est l’angle d’oscillation d’un arc. Cet angle spécifiera jusqu’où, en termes d’angle, le long du chemin circulaire supposé l’arc sera prolongé. L’extension à partir de l’angle de départ sera toujours dans le sens horaire autour du cercle supposé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée y en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

