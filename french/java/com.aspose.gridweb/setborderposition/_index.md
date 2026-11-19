---
title: "SetBorderPosition"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la position de bordure à définir pour une plage de cellules."
type: docs
url: /fr/java/com.aspose.gridweb/setborderposition/
---

**Inheritance:**
java.lang.Object
```
public final class SetBorderPosition
```

Représente la position de bordure à définir pour une plage de cellules.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, GridWeb1.getWorkSheets().get(0).getCells().get(0, 0).getStyle().getLeftBorderStyle());
```
## Champs

| Champ | Description |
| --- | --- |
| [BOTTOM](#BOTTOM) | Bordure inférieure |
| [CROSS](#CROSS) | Bordures croisées |
| [HORIZONTAL_MIDDLE](#HORIZONTAL-MIDDLE) | Bordure inférieure |
| [LEFT](#LEFT) | Bordure gauche |
| [NONE](#NONE) | Pas de bordures |
| [OUTLINE](#OUTLINE) | Bordures VerticalMiddle |
| [RIGHT](#RIGHT) | Bordure droite |
| [TOP](#TOP) | Bordure supérieure |
| [VERTICAL_MIDDLE](#VERTICAL-MIDDLE) | Bordures HorizontalMiddle |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BOTTOM {#BOTTOM}
```
public static final int BOTTOM
```


Bordure inférieure

### CROSS {#CROSS}
```
public static final int CROSS
```


Bordures croisées

### HORIZONTAL_MIDDLE {#HORIZONTAL-MIDDLE}
```
public static final int HORIZONTAL_MIDDLE
```


Bordure inférieure

### LEFT {#LEFT}
```
public static final int LEFT
```


Bordure gauche

### NONE {#NONE}
```
public static final int NONE
```


Pas de bordures

### OUTLINE {#OUTLINE}
```
public static final int OUTLINE
```


Bordures VerticalMiddle

### RIGHT {#RIGHT}
```
public static final int RIGHT
```


Bordure droite

### TOP {#TOP}
```
public static final int TOP
```


Bordure supérieure

### VERTICAL_MIDDLE {#VERTICAL-MIDDLE}
```
public static final int VERTICAL_MIDDLE
```


Bordures HorizontalMiddle

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

