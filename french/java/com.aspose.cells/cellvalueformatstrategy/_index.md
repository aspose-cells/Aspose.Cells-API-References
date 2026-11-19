---
title: "CellValueFormatStrategy"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie comment appliquer le style à la valeur de la cellule."
type: docs
url: /fr/java/com.aspose.cells/cellvalueformatstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CellValueFormatStrategy
```

Spécifie comment appliquer le style à la valeur de la cellule.
## Champs

| Champ | Description |
| --- | --- |
| [CELL_STYLE](#CELL-STYLE) | Uniquement formaté avec le style original de la cellule. |
| [DISPLAY_STRING](#DISPLAY-STRING) | Obtient la chaîne affichée dans MS Excel. |
| [DISPLAY_STYLE](#DISPLAY-STYLE) | Formaté avec le style affiché de la cellule. |
| [NONE](#NONE) | Non formaté. |
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
### CELL_STYLE {#CELL-STYLE}
```
public static final int CELL_STYLE
```


Uniquement formaté avec le style original de la cellule.

### DISPLAY_STRING {#DISPLAY-STRING}
```
public static final int DISPLAY_STRING
```


Obtient la chaîne affichée dans MS Excel. La principale différence avec [DISPLAY\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#DISPLAY-STYLE) est que cette option prend également en compte l'effet de la largeur de colonne. Si la largeur de colonne est trop petite pour afficher la chaîne formatée complètement, "\#" peut être affiché, comme le fait MS Excel.

### DISPLAY_STYLE {#DISPLAY-STYLE}
```
public static final int DISPLAY_STYLE
```


Formaté avec le style affiché de la cellule.

### NONE {#NONE}
```
public static final int NONE
```


Non formaté.

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

