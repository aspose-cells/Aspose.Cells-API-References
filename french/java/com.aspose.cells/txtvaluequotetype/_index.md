---
title: "TxtValueQuoteType"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie le type d'utilisation des guillemets pour les valeurs dans les fichiers au format texte."
type: docs
url: /fr/java/com.aspose.cells/txtvaluequotetype/
---

**Inheritance:**
java.lang.Object
```
public final class TxtValueQuoteType
```

Spécifie le type d'utilisation des guillemets pour les valeurs dans les fichiers au format texte.
## Champs

| Champ | Description |
| --- | --- |
| [ALWAYS](#ALWAYS) | Toutes les valeurs seront toujours entre guillemets. |
| [MINIMUM](#MINIMUM) | Entourez de guillemets les valeurs uniquement si nécessaire. |
| [NEVER](#NEVER) | Toutes les valeurs ne seront pas entre guillemets. |
| [NORMAL](#NORMAL) | Toutes les valeurs contenant des caractères spéciaux tels que le guillemet, le caractère séparateur seront entre guillemets. |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


Toutes les valeurs seront toujours entre guillemets.

### MINIMUM {#MINIMUM}
```
public static final int MINIMUM
```


Entourez de guillemets les valeurs uniquement si nécessaire. Par exemple, si une valeur contient un guillemet mais que le guillemet n'est pas au début de cette valeur, cette valeur ne sera pas entre guillemets.

### NEVER {#NEVER}
```
public static final int NEVER
```


Toutes les valeurs ne seront pas entre guillemets. Le fichier texte exporté avec ce type peut ne pas être relu correctement parce que les guillemets nécessaires sont absents.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Toutes les valeurs contenant des caractères spéciaux tels que les guillemets, le caractère séparateur seront entre guillemets. Même comportement que celui de MS Excel lors de l'exportation d'un fichier texte.

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

