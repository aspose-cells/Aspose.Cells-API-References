---
title: "RevisionCustomView"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un enregistrement de révision d'ajout ou de suppression d'une vue personnalisée au classeur"
type: docs
url: /fr/java/com.aspose.cells/revisioncustomview/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCustomView extends Revision
```

Représente un enregistrement de révision d'ajout ou de suppression d'une vue personnalisée au classeur
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Obtient le type d'action. |
| [getClass()](#getClass--) |  |
| [getGuid()](#getGuid--) | Obtient l'identifiant unique global de la vue personnalisée. |
| [getId()](#getId--) | Obtient le numéro de cette révision. |
| [getType()](#getType--) | Obtient le type de révision. |
| [getWorksheet()](#getWorksheet--) | Obtient la feuille de calcul. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Obtient le type d'action.

Voir [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Obtient l'identifiant unique global de la vue personnalisée.

**Returns:**
java.util.UUID
### getId() {#getId--}
```
public int getId()
```


Obtient le numéro de cette révision.

**Remarks**

Zéro signifie que cette révision ne contient pas d'ID.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Obtient le type de révision.

Voir [RevisionType](../../com.aspose.cells/revisiontype).

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtient la feuille de calcul.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

