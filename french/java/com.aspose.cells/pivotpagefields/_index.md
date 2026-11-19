---
title: "PivotPageFields"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les éléments de page pivot si la source de données du tableau croisé dynamique est des plages de consolidation."
type: docs
url: /fr/java/com.aspose.cells/pivotpagefields/
---

**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```

Représente les éléments de page pivot si la source de données du tableau croisé dynamique est des plages de consolidation. Il ne peut contenir que jusqu'à 4 éléments.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | Représente les éléments de champ de page pivot. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | Définit quelle étiquette d'élément dans chaque champ de page utiliser pour identifier la plage de données. |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | Ajoute un champ de page. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | Obtient le nombre de champs de page. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```


Représente les éléments de champ de page pivot.

### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```


Définit quelle étiquette d'élément dans chaque champ de page utiliser pour identifier la plage de données. pageItemIndex.Length doit être égal à PageFieldCount, veuillez donc ajouter d'abord le champ de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rangeIndex | int | L'index de la plage de données de consolidation. |
| pageItemIndex | int[] | L'index de l'élément de page dans chaque champ de page. pageItemIndex[2] = 1 signifie que le deuxième élément du troisième champ est utilisé pour identifier cette plage. pageItemIndex[1] = -1 signifie qu'aucun élément du deuxième champ n'est utilisé pour identifier cette plage et MS créera automatiquement un élément "blank" dans le deuxième champ pour identifier cette plage. |

### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```


Ajoute un champ de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pageItems | java.lang.String[] | Étiquette d'élément de champ de page |

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
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```


Obtient le nombre de champs de page.

**Returns:**
int
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

