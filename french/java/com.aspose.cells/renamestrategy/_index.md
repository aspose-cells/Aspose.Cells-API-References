---
title: "RenameStrategy"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Option de stratégie pour les noms de colonnes en double."
type: docs
url: /fr/java/com.aspose.cells/renamestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```

Option de stratégie pour les noms de colonnes en double.

**Remarks**

Lors du traitement de données avec des en‑têtes, certains scénarios exigent que les en‑têtes ne soient pas dupliquées pour toutes les colonnes. Par exemple, lors de l'exportation de données vers un datatable et que l'en‑tête doit être utilisé comme nom de colonne du datatable, les valeurs dupliquées de l'en‑tête sont invalides. Pour ce type de situation, l'utilisateur peut déterminer comment les gérer en spécifiant cette stratégie.
## Champs

| Champ | Description |
| --- | --- |
| [DIGIT](#DIGIT) | Nommé avec un chiffre. |
| [EXCEPTION](#EXCEPTION) | Lance une exception. |
| [LETTER](#LETTER) | Nommé avec une lettre.. |
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
### DIGIT {#DIGIT}
```
public static final int DIGIT
```


Nommé avec un chiffre. Les noms dupliqués deviendront ...1, ...2, etc.

### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```


Lance une exception.

### LETTER {#LETTER}
```
public static final int LETTER
```


Nommé avec une lettre.. Les noms dupliqués deviendront ...A, ...B, etc.

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

