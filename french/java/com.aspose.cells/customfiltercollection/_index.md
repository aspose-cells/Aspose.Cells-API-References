---
title: "CustomFilterCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les filtres personnalisés."
type: docs
url: /fr/java/com.aspose.cells/customfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CustomFilterCollection extends CollectionBase
```

Représente les filtres personnalisés.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CustomFilterCollection()](#CustomFilterCollection--) | Construit une nouvelle instance. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-java.lang.Object-boolean-int-java.lang.Object-) | Filtre une liste avec des critères personnalisés. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient le filtre personnalisé à l'index spécifié. |
| [getAnd()](#getAnd--) | Indique si les deux critères ont une relation "et". |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à l'index spécifié. |
| [setAnd(boolean value)](#setAnd-boolean-) | Indique si les deux critères ont une relation "et". |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFilterCollection() {#CustomFilterCollection--}
```
public CustomFilterCollection()
```


Construit une nouvelle instance.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez définir FilterColumn.FilterType sur FilterType.CustomFilters puis obtenir FilterColumn.CustomFilters. Cette propriété sera supprimée 12 mois après juin 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

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
### custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Filtre une liste avec des critères personnalisés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Le type d'opérateur de filtre. |
| criteria1 | java.lang.Object | Le critère personnalisé |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Le type d'opérateur de filtre. |
| criteria2 | java.lang.Object | Le critère personnalisé |

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
public CustomFilter get(int index)
```


Obtient le filtre personnalisé à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

**Returns:**
[CustomFilter](../../com.aspose.cells/customfilter) - 
### getAnd() {#getAnd--}
```
public boolean getAnd()
```


Indique si les deux critères ont une relation "et".

**Returns:**
boolean
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

### setAnd(boolean value) {#setAnd-boolean-}
```
public void setAnd(boolean value)
```


Indique si les deux critères ont une relation "et".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

