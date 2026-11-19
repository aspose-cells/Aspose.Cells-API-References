---
title: "RevisionQueryTable"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une révision d'une modification de champ de tableau de requête."
type: docs
url: /fr/java/com.aspose.cells/revisionquerytable/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionQueryTable extends Revision
```

Représente une révision d'une modification de champ de tableau de requête.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellArea()](#getCellArea--) | Obtient l'emplacement de la table de requête affectée. |
| [getClass()](#getClass--) |  |
| [getFieldId()](#getFieldId--) | Obtient l'ID du champ de la table de requête spécifique qui a été supprimé. |
| [getId()](#getId--) | Obtient le numéro de cette révision. |
| [getType()](#getType--) | Représente le type de la révision. |
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
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Obtient l'emplacement de la table de requête affectée.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFieldId() {#getFieldId--}
```
public int getFieldId()
```


Obtient l'ID du champ de la table de requête spécifique qui a été supprimé.

**Returns:**
int
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


Représente le type de la révision.

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

