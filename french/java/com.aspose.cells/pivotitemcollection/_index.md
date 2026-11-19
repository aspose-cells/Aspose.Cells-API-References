---
title: "PivotItemCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente tous les objets dans le PivotField."
type: docs
url: /fr/java/com.aspose.cells/pivotitemcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotItemCollection extends CollectionBase
```

Représente tous les objets [PivotItem](../../com.aspose.cells/pivotitem) dans le PivotField.
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [changeitemsOrder(int sourceIndex, int destIndex)](#changeitemsOrder-int-int-) | Modifie directement l'ordre des deux éléments. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'objet PivotItem à l'index spécifié. |
| [get(String itemValue)](#get-java.lang.String-) | Obtient le [PivotItem](../../com.aspose.cells/pivotitem) par le nom spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [hideAllDetail(boolean isHiddenDetail)](#hideAllDetail-boolean-) | Définit s'il faut masquer tous les détails de tous les PivotItems dans un champ pivot. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à l'index spécifié. |
| [swapItem(int index1, int index2)](#swapItem-int-int-) | Échange directement deux éléments. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Ajoute un élément à l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | L'objet à ajouter à l'instance CollectionBase. |

**Returns:**
int - La position dans laquelle le nouvel élément a été inséré.
### changeitemsOrder(int sourceIndex, int destIndex) {#changeitemsOrder-int-int-}
```
public void changeitemsOrder(int sourceIndex, int destIndex)
```


Modifie directement l'ordre des deux éléments.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotItemCollection.SwapItem(). Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceIndex | int | L'index actuel |
| destIndex | int | L'index de destination |

### clear() {#clear--}
```
public void clear()
```


Supprime tous les objets de l'instance CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Renvoie si l'instance contient cet objet

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | objet de test |

**Returns:**
boolean - Si l'instance contient cet objet
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
public PivotItem get(int index)
```


Obtient l'objet PivotItem à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
### get(String itemValue) {#get-java.lang.String-}
```
public PivotItem get(String itemValue)
```


Obtient le [PivotItem](../../com.aspose.cells/pivotitem) par le nom spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| itemValue | java.lang.String |  |

**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
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


Obtient le nombre d'éléments contenus dans l'instance CollectionBase.

**Returns:**
int - Le nombre d'éléments contenus dans l'instance CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetail(boolean isHiddenDetail) {#hideAllDetail-boolean-}
```
public void hideAllDetail(boolean isHiddenDetail)
```


Définit s'il faut masquer tous les détails de tous les PivotItems dans un champ pivot. C’est le repliement/expansion de ce champ.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser les méthodes PivotField.HideAllDetails() et ShowAllDetails(). Cette méthode sera supprimée 12 mois plus tard, à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isHiddenDetail | boolean | Indique si le détail du champ pivot doit être masqué. |

### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Détermine l'index d'un élément spécifique dans l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |

**Returns:**
int - L'index de la valeur si elle est trouvée dans la liste ; sinon, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Renvoie un énumérateur qui parcourt l'instance CollectionBase.

**Returns:**
java.util.Iterator - Un itérateur pour l'instance CollectionBase.
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


Supprime l'élément à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index basé sur zéro de l'élément à supprimer. |

### swapItem(int index1, int index2) {#swapItem-int-int-}
```
public void swapItem(int index1, int index2)
```


Échange directement deux éléments.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index1 | int |  |
| index2 | int |  |

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

