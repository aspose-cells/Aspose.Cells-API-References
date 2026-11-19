---
title: "PivotFilterCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une collection de tous les PivotFilters."
type: docs
url: /fr/java/com.aspose.cells/pivotfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```

Représente une collection de tous les PivotFilters.
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | Ajoute un objet PivotFilter au type spécifique |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtre par réglage de date du champ pivot de ligne ou de colonne. |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | Filtre par légendes du champ pivot de ligne ou de colonne. |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | Filtre par valeurs du champ pivot de données. |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | Filtre par valeurs du champ pivot de données. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | Efface le PivotFilter du PivotField spécifique |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'objet pivotfilter à l'index spécifique. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```


Ajoute un objet PivotFilter au type spécifique

**Remarks**

NOTE : Cette méthode est désormais obsolète. À la place, veuillez utiliser les méthodes PivotFilterCollection.AddValueFilter(), AddTop10Filter(), AddLabelFilter() et AddDateFilter(). Cette méthode sera supprimée 12 mois après, depuis novembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | l'index du PivotField |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). le type de PivotFilter |

**Returns:**
int - l'index de l'objet PivotFilter dans cette PivotFilterCollection.
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
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```


Filtre par réglage de date du champ pivot de ligne ou de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | L'index du champ dans la source. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Le type de filtrage des données. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | L'étiquette de date de la condition de filtrage |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | L'étiquette de date supérieure de la condition de filtrage entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```


Filtre par légendes du champ pivot de ligne ou de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | L'index du champ dans la source. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Le type de filtrage des données. |
| label1 | java.lang.String | L'étiquette de la condition de filtrage |
| label2 | java.lang.String | L'étiquette supérieure de la condition de filtre entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtre par valeurs du champ pivot de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | L'index du champ dans la source. |
| valueFieldIndex | int | L'index du champ de données dans la région de données. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Le type de filtrage des données. Peut uniquement être Count,Sum et Percent. |
| isTop | boolean | Indique si le filtre provient du haut ou du bas |
| itemCount | int | Le nombre d'éléments |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```


Filtre par valeurs du champ pivot de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | L'index du champ dans la source. |
| valueFieldIndex | int | L'index du champ de valeur dans la région de valeur. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Le type de filtrage des données. |
| value1 | double | La valeur de la condition de filtre |
| value2 | double | La valeur supérieure de la condition de filtre entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```


Supprime tous les objets de l'instance CollectionBase.

### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```


Efface le PivotFilter du PivotField spécifique

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | l'index du PivotField |

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
public PivotFilter get(int index)
```


Obtient l'objet pivotfilter à l'index spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
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

