---
title: "ReserveMissingPivotItemType"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente comment conserver les éléments de tableau croisé dynamique manquants."
type: docs
url: /fr/java/com.aspose.cells/reservemissingpivotitemtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReserveMissingPivotItemType
```

Représente comment conserver les éléments de tableau croisé dynamique manquants.
## Champs

| Champ | Description |
| --- | --- |
| [ALL](#ALL) | Réserve tous les éléments manquants. |
| [DEFAULT](#DEFAULT) | Supprime les anciens éléments manquants du tableau croisé dynamique et réserve les éléments supprimés de la nouvelle source de données comme éléments manquants. |
| [NONE](#NONE) | Supprime tous les éléments manquants du tableau croisé dynamique. |
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
### ALL {#ALL}
```
public static final int ALL
```


Réserve tous les éléments manquants.

**Remarks**

Dans Excel, tant qu’Excel n’est pas fermé, les éléments manquants générés lors du premier rafraîchissement du tableau croisé dynamique seront conservés, même si vous rafraîchissez à plusieurs reprises.

### DEFAULT {#DEFAULT}
```
public static final int DEFAULT
```


Supprime les anciens éléments manquants du tableau croisé dynamique et réserve les éléments supprimés de la nouvelle source de données comme éléments manquants.

### NONE {#NONE}
```
public static final int NONE
```


Supprime tous les éléments manquants du tableau croisé dynamique.

**Remarks**

L'ordre des anciens éléments de tableau croisé dynamique manquants sera ignoré.

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

