---
title: "SessionMode"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le mode de session de la grille."
type: docs
url: /fr/java/com.aspose.gridweb/sessionmode/
---

**Inheritance:**
java.lang.Object
```
public final class SessionMode
```

Représente le mode de session de la grille.
## Champs

| Champ | Description |
| --- | --- |
| [CUSTOM](#CUSTOM) | Utilise l'événement LoadCustomData pour charger les données de la feuille du grid manuellement. |
| [FILE](#FILE) | Utilise le fichier système pour stocker/récupérer automatiquement les données de la feuille du grid, l'utilisateur doit définir SessionStorePath pour spécifier le répertoire du fichier. |
| [SESSION](#SESSION) | Utilise la session système pour stocker/récupérer automatiquement les données de la feuille du grid. |
| [VIEW_STATE](#VIEW-STATE) | Utilise le viewstate de la page pour stocker/récupérer automatiquement les données de la feuille du grid. |
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
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Utilise l'événement LoadCustomData pour charger les données de la feuille du grid manuellement. Et utilise l'événement SheetDataUpdated pour enregistrer les données de la feuille du grid.

### FILE {#FILE}
```
public static final int FILE
```


Utilise le fichier système pour stocker/récupérer automatiquement les données de la feuille du grid, l'utilisateur doit définir SessionStorePath pour spécifier le répertoire du fichier.

### SESSION {#SESSION}
```
public static final int SESSION
```


Utilise la session système pour stocker/récupérer automatiquement les données de la feuille du grid.

### VIEW_STATE {#VIEW-STATE}
```
public static final int VIEW_STATE
```


Utilise le viewstate de la page pour stocker/récupérer automatiquement les données de la feuille du grid.

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

