---
title: "NameCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une collection de tous les objets dans la feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/namecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```

Représente une collection de tous les objets [Name](../../com.aspose.cells/name) dans la feuille de calcul.
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String text)](#add-java.lang.String-) | Définit un nouveau nom. |
| [clear()](#clear--) | Supprime tous les noms définis qui ne sont pas référencés par les formules et la source de données. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | Obtient tous les noms définis par portée. |
| [get(int index)](#get-int-) | Obtient l'élément [Name](../../com.aspose.cells/name) à l'index spécifié. |
| [get(String text)](#get-java.lang.String-) | Obtient l'élément [Name](../../com.aspose.cells/name) avec le nom spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | Supprime le nom. |
| [remove(String[] names)](#remove-java.lang.String---) | Supprime un tableau de noms. |
| [removeAt(int index)](#removeAt-int-) | Supprime le nom à l'index spécifié. |
| [removeDuplicateNames()](#removeDuplicateNames--) | Supprime les noms définis en double |
| [sort()](#sort--) | Trie les noms définis. |
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
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```


Définit un nouveau nom.

**Remarks**

Le nom ne peut pas contenir d'espaces et ne peut pas ressembler à des références de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| texte | java.lang.String | Le texte à utiliser comme nom. |

**Returns:**
int - index de l'objet [Name](../../com.aspose.cells/name).
### clear() {#clear--}
```
public void clear()
```


Supprime tous les noms définis qui ne sont pas référencés par les formules et la source de données. Si le nom défini est référencé, nous ne faisons que définir Name.ReferTo sur null et les masquer.

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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```


Obtient tous les noms définis par portée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype). Le type de portée. |
| sheetIndex | int | L'index de la feuille. N'affecte que lorsque le type de portée est [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET). |

**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```


Obtient l'élément [Name](../../com.aspose.cells/name) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```


Obtient l'élément [Name](../../com.aspose.cells/name) avec le nom spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| texte | java.lang.String | Texte du nom. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element with the specified name.
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




### remove(String text) {#remove-java.lang.String-}
```
public void remove(String text)
```


Supprime le nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| texte | java.lang.String | Le texte du nom. |

### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Supprime un tableau de noms.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| noms | java.lang.String[] | Le texte des noms. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime le nom à l'index spécifié.

**Remarks**

Veuillez vous assurer que le nom n'est pas référencé par les autres formules avant d'appeler la méthode. Et si le nom est référencé, définir Name.RefersTo sur null est préférable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | indice du Name à supprimer. |

### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```


Supprime les noms définis en double

### sort() {#sort--}
```
public void sort()
```


Trie les noms définis.

**Remarks**

Si vous créez un grand nombre de plages nommées dans le fichier Excel, veuillez appeler cette méthode après la création de toutes les plages nommées et avant l'enregistrement.

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

