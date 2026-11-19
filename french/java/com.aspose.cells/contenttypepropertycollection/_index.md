---
title: "ContentTypePropertyCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Une collection d'objets qui représentent des informations supplémentaires."
type: docs
url: /fr/java/com.aspose.cells/contenttypepropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ContentTypePropertyCollection extends CollectionBase
```

Une collection d'objets [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) qui représentent des informations supplémentaires.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Add a new property.
          workbook.getContentTypeProperties().add("Admin", "Aspose", "text");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Ajoute des informations de propriété de type de contenu. |
| [add(String name, String value, String type)](#add-java.lang.String-java.lang.String-java.lang.String-) | Ajoute des informations de propriété de type de contenu. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient la propriété de type de contenu par l'index spécifié. |
| [get(String name)](#get-java.lang.String-) | Obtient la propriété de type de contenu par le nom de la propriété. |
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
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public int add(String name, String value)
```


Ajoute des informations de propriété de type de contenu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété de type de contenu. |
| valeur | java.lang.String | La valeur de la propriété de type de contenu. |

**Returns:**
int
### add(String name, String value, String type) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String name, String value, String type)
```


Ajoute des informations de propriété de type de contenu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété de type de contenu. |
| valeur | java.lang.String | La valeur de la propriété de type de contenu. |
| type | java.lang.String | Le type de la propriété de type de contenu. |

**Returns:**
int
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
public ContentTypeProperty get(int index)
```


Obtient la propriété de type de contenu par l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

**Returns:**
[ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) - The content type property
### get(String name) {#get-java.lang.String-}
```
public ContentTypeProperty get(String name)
```


Obtient la propriété de type de contenu par le nom de la propriété.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |

**Returns:**
[ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) - The content type property
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

