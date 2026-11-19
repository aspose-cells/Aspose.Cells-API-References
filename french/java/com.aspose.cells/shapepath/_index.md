---
title: "ShapePath"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un chemin de création composé d'une série de lignes et de courbes de déplacement qui, combinées, formeront une forme géométrique."
type: docs
url: /fr/java/com.aspose.cells/shapepath/
---

**Inheritance:**
java.lang.Object
```
public class ShapePath
```

Représente un chemin de création composé d'une série de déplacements, de lignes et de courbes qui, une fois combinés, formeront une forme géométrique.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ShapePath()](#ShapePath--) | Initialise une nouvelle instance de la classe [ShapePath](../../com.aspose.cells/shapepath). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | Ajoute un arc elliptique à la figure actuelle. |
| [close()](#close--) | Ferme la figure actuelle et démarre une nouvelle figure. |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | Ajoute une courbe cubique B\u8305zier à la figure actuelle. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | Obtient la hauteur de ce chemin en pixels. |
| [getPathSegementList()](#getPathSegementList--) | Obtient la liste [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) |
| [getPathSegments()](#getPathSegments--) | Obtient la liste [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) |
| [getWidthPixel()](#getWidthPixel--) | Obtient la largeur de ce chemin en pixels. |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | Ajoute un segment de ligne à la figure actuelle. |
| [moveTo(float x, float y)](#moveTo-float-float-) | Démarre une nouvelle figure à partir du point spécifié sans fermer la figure actuelle. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Obtient la hauteur de ce chemin en pixels. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Obtient la largeur de ce chemin en pixels. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```


Initialise une nouvelle instance de la classe [ShapePath](../../com.aspose.cells/shapepath).

### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```


Ajoute un arc elliptique à la figure actuelle. Le point de départ est le point final de la figure actuelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| wR | float | La demi-largeur de la zone rectangulaire de \\u9225\\u5b27\\u20ac\\u5aa1he ellipse qui trace l'arc (Unité : Pixel). |
| hR | float | La demi-hauteur de la zone rectangulaire de \\u9225\\u5b27\\u20ac\\u5aa1he ellipse qui trace l'arc (Unité : Pixel). |
| stAng | float | L'angle de départ de l'arc, mesuré en degrés dans le sens horaire à partir de l'axe des x (Unité : Degré). Cet angle spécifiera quel angle le long du chemin circulaire supposé sera utilisé comme position de départ pour tracer l'arc. Cet angle de départ sera verrouillé à la dernière position connue du stylo dans le chemin de forme. Garantissant ainsi un chemin de forme continu. |
| swAng | float | L'angle d'oscillation pour un arc. Cet angle spécifiera jusqu'où, en termes d'angle, le long du chemin circulaire supposé l'arc sera prolongé. L'extension à partir de l'angle de départ sera toujours dans le sens horaire autour du cercle supposé. (Unité : Degré) |

### close() {#close--}
```
public void close()
```


Ferme la figure actuelle et démarre une nouvelle figure. Si la figure actuelle contient une séquence de lignes et de courbes connectées, la méthode ferme la boucle en reliant une ligne du point final au point de départ.

### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```


Ajoute une courbe cubique B\\u8305zier à la figure actuelle. Le point de départ est le point final de la figure actuelle. Unité : Pixel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ctrX1 | float | La coordonnée x du premier point de contrôle de la courbe (Unité : Pixel). |
| ctrY1 | float | La coordonnée y du premier point de contrôle de la courbe (Unité : Pixel). |
| ctrX2 | float | La coordonnée x du deuxième point de contrôle de la courbe (Unité : Pixel). |
| ctrY2 | float | La coordonnée y du deuxième point de contrôle de la courbe (Unité : Pixel). |
| endX | float | La coordonnée x du point final de la courbe (Unité : Pixel). |
| endY | float | La coordonnée y du point final de la courbe (Unité : Pixel). |

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
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Obtient la hauteur de ce chemin en pixels.

**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```


Obtient la liste [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ShapePath.PathSegments. Cette propriété sera supprimée 12 mois plus tard, depuis juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getPathSegments() {#getPathSegments--}
```
public ShapeSegmentPathCollection getPathSegments()
```


Obtient la liste [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Obtient la largeur de ce chemin en pixels.

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


Ajoute un segment de ligne à la figure actuelle. Le point de départ est le point final de la figure actuelle. Unité : Pixel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| x | float | La coordonnée x du point final du segment de ligne (Unité : Pixel). |
| y | float | La coordonnée y du point final du segment de ligne (Unité : Pixel). |

### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```


Commence une nouvelle figure à partir du point spécifié sans fermer la figure actuelle. Tous les points suivants ajoutés au chemin sont ajoutés à cette nouvelle figure. Unité : Pixel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| x | float | La coordonnée x du point de départ de la figure (Unité : Pixel). |
| y | float | La coordonnée y du point de départ de la figure (Unité : Pixel). |

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


Obtient la hauteur de ce chemin en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Obtient la largeur de ce chemin en pixels.

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

