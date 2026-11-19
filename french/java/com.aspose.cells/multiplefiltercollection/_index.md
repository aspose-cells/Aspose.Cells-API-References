---
title: "MultipleFilterCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la collection de filtres multiples."
type: docs
url: /fr/java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

Représente la collection de filtres multiples.

**Remarks**

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser [FilterValueCollection](../../com.aspose.cells/filtervaluecollection). Cette propriété sera supprimée 12 mois plus tard, à compter de juin 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | Construit une nouvelle instance. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | Ajoute une valeur de critère de filtre de date. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | Ajoute une valeur de critère de filtre de date et heure. |
| [add(String filter)](#add-java.lang.String-) | Ajoute un critère de filtre d'étiquette. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) ou une valeur de chaîne. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre de valeurs du filtre. |
| [getMatchBlank()](#getMatchBlank--) | Indique s'il faut filtrer par valeur vide. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Obtenez l'énumérateur pour la valeur du filtre, |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | Indique s'il faut filtrer par valeur vide. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


Construit une nouvelle instance.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez définir FilterColumn.FilterType sur FilterType.MultipleFilters puis obtenir FilterColumn.MultipleFilters. Cette propriété sera supprimée 12 mois plus tard, à compter de juin 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


Ajoute une valeur de critère de filtre de date.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Le type de filtre de date. |
| année | int | L'année. |
| mois | int | Le mois. |
| jour | int | Le jour. |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


Ajoute une valeur de critère de filtre de date et heure.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Le type de filtre de date. |
| année | int | L'année. |
| mois | int | Le mois. |
| jour | int | Le jour. |
| heure | int | L'heure. |
| minute | int | La minute. |
| seconde | int | La seconde. |

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


Ajoute un critère de filtre d'étiquette.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filtre | java.lang.String | Les données du filtre. |

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
public Object get(int index)
```


Obtient [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) ou une valeur de chaîne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
java.lang.Object -
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


Obtient le nombre de valeurs du filtre.

**Returns:**
int
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


Indique s'il faut filtrer par valeur vide.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtenez l'énumérateur pour la valeur du filtre,

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMatchBlank(boolean value) {#setMatchBlank-boolean-}
```
public void setMatchBlank(boolean value)
```


Indique s'il faut filtrer par valeur vide.

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

