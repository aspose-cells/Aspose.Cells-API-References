---
title: "GridValidationCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.gridweb/gridvalidationcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```

Encapsule une collection d'objets [GridValidation](../../com.aspose.gridweb/gridvalidation).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add()](#add--) | Ajoute un [GridValidation](../../com.aspose.gridweb/gridvalidation) à la collection. |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | Ajoute une validation de données à la collection. |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | Ajoute un [GridValidation](../../com.aspose.gridweb/gridvalidation) à la collection. |
| [add(int row, int column)](#add-int-int-) | Ajoute un [GridValidation](../../com.aspose.gridweb/gridvalidation) à la collection. La validation est appliquée à la cellule spécifiée. |
| [add(String cellname)](#add-java.lang.String-) | Ajoute un [GridValidation](../../com.aspose.gridweb/gridvalidation) à la collection. La validation est appliquée à la cellule spécifiée. |
| [clear()](#clear--) | Efface toutes les validations. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [GridValidation](../../com.aspose.gridweb/gridvalidation) à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient la taille de l'énumérateur |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | Obtient la validation appliquée à la cellule donnée. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime la validation à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```


Ajoute un [GridValidation](../../com.aspose.gridweb/gridvalidation) à la collection.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode GridValidationCollection.Add(row,col). Cette propriété sera supprimée 12 mois plus tard à compter de JANVIER 2015. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```


Ajoute une validation de données à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | La zone contient cette validation. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```


Ajoute un [GridValidation](../../com.aspose.gridweb/gridvalidation) à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | Un objet de validation. |

**Returns:**
int - index de l'objet [GridValidation](../../com.aspose.gridweb/gridvalidation).
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```


Ajoute un [GridValidation](../../com.aspose.gridweb/gridvalidation) à la collection. La validation est appliquée à la cellule spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```


Ajoute un [GridValidation](../../com.aspose.gridweb/gridvalidation) à la collection. La validation est appliquée à la cellule spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellname | java.lang.String | le nom de la cellule. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```


Efface toutes les validations.

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
### get(int index) {#get-int-}
```
public GridValidation get(int index)
```


Obtient l'élément [GridValidation](../../com.aspose.gridweb/gridvalidation) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtient la taille de l'énumérateur

**Returns:**
int
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```


Obtient la validation appliquée à la cellule donnée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime la validation à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

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

