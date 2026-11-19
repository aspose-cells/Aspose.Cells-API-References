---
title: "RowColumnEventArgs"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Fournit des données pour les événements ligne/colonne."
type: docs
url: /fr/java/com.aspose.gridweb/rowcolumneventargs/
---

**Inheritance:**
java.lang.Object
```
public class RowColumnEventArgs
```

Fournit des données pour les événements ligne/colonne.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgument()](#getArgument--) | L'argument de l'événement. |
| [getClass()](#getClass--) |  |
| [getNum()](#getNum--) | Le numéro de ligne ou de colonne, commence à zéro. |
| [getType()](#getType--) | Le type de ligne ou de colonne. |
| [hashCode()](#hashCode--) |  |
| [isCancel()](#isCancel--) | devons‑nous annuler l'opération. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rejectOperation()](#rejectOperation--) | Appelez cette méthode dans les gestionnaires d'événements RowDeleting/ColumnDeleting pour annuler les opérations de suppression. |
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
### getArgument() {#getArgument--}
```
public Object getArgument()
```


L'argument de l'événement.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getNum() {#getNum--}
```
public int getNum()
```


Le numéro de ligne ou de colonne, commence à zéro.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Le type de ligne ou de colonne.

Voir [RowColumnType](../../com.aspose.gridweb/rowcolumntype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCancel() {#isCancel--}
```
public boolean isCancel()
```


devons‑nous annuler l'opération.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rejectOperation() {#rejectOperation--}
```
public void rejectOperation()
```


Appelez cette méthode dans les gestionnaires d'événements RowDeleting/ColumnDeleting pour annuler les opérations de suppression.

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

