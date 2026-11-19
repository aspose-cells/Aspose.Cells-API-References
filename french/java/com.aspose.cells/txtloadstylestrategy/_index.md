---
title: "TxtLoadStyleStrategy"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie comment appliquer le style aux valeurs analysées lors de la conversion d'une chaîne en nombre ou en date/heure."
type: docs
url: /fr/java/com.aspose.cells/txtloadstylestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```

Spécifie comment appliquer le style aux valeurs analysées lors de la conversion d'une chaîne en nombre ou en date/heure.
## Champs

| Champ | Description |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | Définissez le style comme nombre/date-heure intégré lorsque la valeur analysée est une valeur numérique/date-heure simple. |
| [EXACT_FORMAT](#EXACT-FORMAT) | Définissez le format personnalisé exact pour la valeur analysée afin que la valeur formatée soit identique à celle de l'entrée d'origine. |
| [NONE](#NONE) | Ne définit pas le style pour la valeur analysée. |
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
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```


Définissez le style comme nombre/date-heure intégré lorsque la valeur analysée est une valeur numérique/date-heure simple.

**Remarks**

Lorsque MS Excel analyse des valeurs date‑heure ou numériques selon l'entrée de l'utilisateur (par exemple un fichier CSV), le formatage de ces valeurs peut être modifié, comme les zéros de tête ou de fin d'un nombre, l'ordre année/mois/jour d'une date‑heure, …etc. Ce type sert à simuler le comportement de MS Excel.

### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```


Définissez le format personnalisé exact pour la valeur analysée afin que la valeur formatée soit identique à celle de l'entrée d'origine.

### NONE {#NONE}
```
public static final int NONE
```


Ne définit pas le style pour la valeur analysée.

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

