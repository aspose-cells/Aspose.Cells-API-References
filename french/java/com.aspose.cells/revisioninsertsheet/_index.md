---
title: "RevisionInsertSheet"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un enregistrement de révision d'une feuille qui a été insérée."
type: docs
url: /fr/java/com.aspose.cells/revisioninsertsheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionInsertSheet extends Revision
```

Représente un enregistrement de révision d'une feuille qui a été insérée.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Obtient le type d'action de la révision. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Obtient le numéro de cette révision. |
| [getName()](#getName--) | Obtient le nom de la feuille de calcul. |
| [getSheetPosition()](#getSheetPosition--) | Obtient la position basée sur zéro de la nouvelle feuille dans la barre d'onglets de feuilles. |
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


Obtient le type d'action de la révision.

Voir [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getId() {#getId--}
```
public int getId()
```


Obtient le numéro de cette révision.

**Remarks**

Zéro signifie que cette révision ne contient pas d'ID.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la feuille de calcul.

**Returns:**
java.lang.String
### getSheetPosition() {#getSheetPosition--}
```
public int getSheetPosition()
```


Obtient la position basée sur zéro de la nouvelle feuille dans la barre d'onglets de feuilles.

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

