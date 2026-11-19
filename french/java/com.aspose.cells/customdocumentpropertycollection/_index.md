---
title: "CustomDocumentPropertyCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Une collection de propriétés de document personnalisées."
type: docs
url: /fr/java/com.aspose.cells/customdocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class CustomDocumentPropertyCollection extends DocumentPropertyCollection
```

Une collection de propriétés de document personnalisées.

**Remarks**

Chaque objet représente une propriété personnalisée d'un document conteneur.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         CustomDocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.Boolean**. |
| [add(String name, DateTime value)](#add-java.lang.String-com.aspose.cells.DateTime-) | Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.DateTime**. |
| [add(String name, double value)](#add-java.lang.String-double-) | Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.Float**. |
| [add(String name, int value)](#add-java.lang.String-int-) | Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.Number**. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.String**. |
| [addLinkToContent(String name, String source)](#addLinkToContent-java.lang.String-java.lang.String-) | Crée une nouvelle propriété de document personnalisée qui lie au contenu. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [contains(String name)](#contains-java.lang.String-) | Renvoie true si une propriété portant le nom spécifié existe dans la collection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Renvoie un objet [DocumentProperty](../../com.aspose.cells/documentproperty) par indice. |
| [get(String name)](#get-java.lang.String-) | Renvoie un objet [DocumentProperty](../../com.aspose.cells/documentproperty) par le nom de la propriété. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Obtient l'indice d'une propriété par son nom. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Supprime une propriété portant le nom spécifié de la collection. |
| [removeAt(int index)](#removeAt-int-) | Supprime une propriété à l'indice spécifié. |
| [toString()](#toString--) |  |
| [updateLinkedPropertyValue()](#updateLinkedPropertyValue--) | Met à jour les valeurs de toutes les propriétés personnalisées qui sont liées au contenu (utilise la valeur de cellule de la plage liée pour mettre à jour la valeur de la propriété personnalisée). |
| [updateLinkedRange()](#updateLinkedRange--) | Met à jour toutes les plages qui sont liées aux propriétés personnalisées (utilise la valeur de la propriété de document personnalisée pour mettre à jour la valeur de cellule de la plage liée). |
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
### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public DocumentProperty add(String name, boolean value)
```


Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.Boolean**.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| valeur | boolean | La valeur de la propriété. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, DateTime value) {#add-java.lang.String-com.aspose.cells.DateTime-}
```
public DocumentProperty add(String name, DateTime value)
```


Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.DateTime**.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| value | [DateTime](../../com.aspose.cells/datetime) | La valeur de la propriété. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public DocumentProperty add(String name, double value)
```


Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.Float**.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| valeur | double | La valeur de la propriété. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, int value) {#add-java.lang.String-int-}
```
public DocumentProperty add(String name, int value)
```


Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.Number**.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| valeur | int | La valeur de la propriété. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public DocumentProperty add(String name, String value)
```


Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.String**.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| valeur | java.lang.String | La valeur de la propriété. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### addLinkToContent(String name, String source) {#addLinkToContent-java.lang.String-java.lang.String-}
```
public DocumentProperty addLinkToContent(String name, String source)
```


Crée une nouvelle propriété de document personnalisée qui lie au contenu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| source | java.lang.String | La source de la propriété. Cela doit être le nom de la plage nommée. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Renvoie true si une propriété portant le nom spécifié existe dans la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété, insensible à la casse. |

**Returns:**
boolean - True si la propriété existe dans la collection ; false sinon.
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
public DocumentProperty get(int index)
```


Renvoie un objet [DocumentProperty](../../com.aspose.cells/documentproperty) par indice.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | Indice basé sur zéro du [DocumentProperty](../../com.aspose.cells/documentproperty) à récupérer. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Renvoie un objet [DocumentProperty](../../com.aspose.cells/documentproperty) par le nom de la propriété.

**Remarks**

Renvoie null si aucune propriété portant le nom spécifié n'est trouvée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété, insensible à la casse, à récupérer. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Obtient l'indice d'une propriété par son nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété, insensible à la casse. |

**Returns:**
int - L'index basé sur zéro. Valeur négative si non trouvé.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Supprime une propriété portant le nom spécifié de la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété, insensible à la casse. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime une propriété à l'indice spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index basé sur zéro. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateLinkedPropertyValue() {#updateLinkedPropertyValue--}
```
public void updateLinkedPropertyValue()
```


Met à jour les valeurs de toutes les propriétés personnalisées qui sont liées au contenu (utilise la valeur de cellule de la plage liée pour mettre à jour la valeur de la propriété personnalisée).

### updateLinkedRange() {#updateLinkedRange--}
```
public void updateLinkedRange()
```


Met à jour toutes les plages qui sont liées aux propriétés personnalisées (utilise la valeur de la propriété de document personnalisée pour mettre à jour la valeur de cellule de la plage liée).

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

