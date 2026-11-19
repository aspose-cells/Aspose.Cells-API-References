---
title: "SheetSet"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Décrit un ensemble de feuilles."
type: docs
url: /fr/java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

Décrit un ensemble de feuilles.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SheetSet(int[] sheetIndexes)](#SheetSet-int---) | Crée un ensemble de feuilles basé sur des index de feuilles exacts. |
| [SheetSet(String[] sheetNames)](#SheetSet-java.lang.String---) | Crée un ensemble de feuilles basé sur des noms de feuilles exacts. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | Obtient un ensemble avec la feuille active du classeur. |
| [getAll()](#getAll--) | Obtient un ensemble avec toutes les feuilles du classeur dans leur ordre d'origine. |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | Obtient un ensemble avec les feuilles visibles du classeur dans leur ordre d'origine. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheetIndexes) {#SheetSet-int---}
```
public SheetSet(int[] sheetIndexes)
```


Crée un ensemble de feuilles basé sur des index de feuilles exacts.

**Remarks**

Si une feuille est rencontrée qui n'est pas dans le classeur, une exception sera levée lors du rendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndexes | int[] | index de feuilles basés sur zéro. |

### SheetSet(String[] sheetNames) {#SheetSet-java.lang.String---}
```
public SheetSet(String[] sheetNames)
```


Crée un ensemble de feuilles basé sur des noms de feuilles exacts.

**Remarks**

Si une feuille est rencontrée qui n'est pas dans le classeur, une exception sera levée lors du rendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetNames | java.lang.String[] | noms de feuilles. |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


Obtient un ensemble avec la feuille active du classeur.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


Obtient un ensemble avec toutes les feuilles du classeur dans leur ordre d'origine.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


Obtient un ensemble avec les feuilles visibles du classeur dans leur ordre d'origine.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

