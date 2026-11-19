---
title: "DefaultStyleSettings"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Paramètres des valeurs par défaut des propriétés de style des classeurs."
type: docs
url: /fr/java/com.aspose.cells/defaultstylesettings/
---

**Inheritance:**
java.lang.Object
```
public class DefaultStyleSettings
```

Paramètres pour les valeurs par défaut des propriétés de style du classeur.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInPreference()](#getBuiltInPreference--) | Indique si la propriété du format numérique est préférable lorsque le style définit à la fois un nombre intégré et un motif personnalisé. |
| [getClass()](#getClass--) |  |
| [getFontName()](#getFontName--) | Obtient le nom de police par défaut pour le classeur |
| [getFontSize()](#getFontSize--) | Obtient la taille de police standard par défaut pour le classeur. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Obtient la valeur par défaut pour l'alignement horizontal |
| [getVerticalAlignment()](#getVerticalAlignment--) | Obtient la valeur par défaut pour l'alignement vertical |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuiltInPreference(boolean value)](#setBuiltInPreference-boolean-) | Indique si la propriété du format numérique est préférable lorsque le style définit à la fois un nombre intégré et un motif personnalisé. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Définit le nom de police par défaut pour le classeur |
| [setFontSize(double value)](#setFontSize-double-) | Définit la taille de police standard par défaut pour le classeur. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Définit la valeur par défaut pour l'alignement horizontal |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Définit la valeur par défaut pour l'alignement vertical |
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
### getBuiltInPreference() {#getBuiltInPreference--}
```
public boolean getBuiltInPreference()
```


Indique si la propriété du format de nombre est préférable lorsque le style définit à la fois un nombre intégré et un modèle personnalisé. La valeur par défaut est false, ce qui signifie qu'en défaut le modèle personnalisé sera utilisé pour formater les valeurs tant qu'il n'est pas vide pour un style.

**Remarks**

Lors du chargement d'un classeur à partir d'un fichier modèle existant, il se peut que le nombre intégré et le modèle personnalisé soient tous deux définis pour un style. Cette propriété détermine si nous devons utiliser le nombre intégré ou le modèle personnalisé lors du formatage des valeurs avec le style.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontName() {#getFontName--}
```
public String getFontName()
```


Obtient le nom de police par défaut pour le classeur

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Obtient la taille de police standard par défaut pour le classeur.

**Returns:**
double
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Obtient la valeur par défaut pour l'alignement horizontal

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Obtient la valeur par défaut pour l'alignement vertical

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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




### setBuiltInPreference(boolean value) {#setBuiltInPreference-boolean-}
```
public void setBuiltInPreference(boolean value)
```


Indique si la propriété du format de nombre est préférable lorsque le style définit à la fois un nombre intégré et un modèle personnalisé. La valeur par défaut est false, ce qui signifie qu'en défaut le modèle personnalisé sera utilisé pour formater les valeurs tant qu'il n'est pas vide pour un style.

**Remarks**

Lors du chargement d'un classeur à partir d'un fichier modèle existant, il se peut que le nombre intégré et le modèle personnalisé soient tous deux définis pour un style. Cette propriété détermine si nous devons utiliser le nombre intégré ou le modèle personnalisé lors du formatage des valeurs avec le style.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Définit le nom de police par défaut pour le classeur

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFontSize(double value) {#setFontSize-double-}
```
public void setFontSize(double value)
```


Définit la taille de police standard par défaut pour le classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Définit la valeur par défaut pour l'alignement horizontal

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Définit la valeur par défaut pour l'alignement vertical

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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

