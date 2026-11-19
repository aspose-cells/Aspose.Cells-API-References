---
title: "XmlMapCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Une collection d'objets qui représentent les informations XmlMap."
type: docs
url: /fr/java/com.aspose.cells/xmlmapcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class XmlMapCollection extends CollectionBase
```

Une collection d'objets [XmlMap](../../com.aspose.cells/xmlmap) qui représentent les informations XmlMap.
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String url)](#add-java.lang.String-) | Ajoutez un [XmlMap](../../com.aspose.cells/xmlmap) via l'url/chemin d'un fichier xml/xsd. |
| [clear()](#clear--) | Supprime tous les XmlMaps. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient le xml map par l'index spécifique. |
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
### add(String url) {#add-java.lang.String-}
```
public int add(String url)
```


Ajoutez un [XmlMap](../../com.aspose.cells/xmlmap) via l'url/chemin d'un fichier xml/xsd.

**Example**

Le code suivant ajoute deux XmlMaps à partir d'un fichier xsd et d'un fichier xml.

```
         Workbook wb = new Workbook();
 
         XmlMapCollection xmlMapCollection = wb.getWorksheets().getXmlMaps();
 
         //Add a XmlMap by a xsd file.
         xmlMapCollection.add("schema.xsd");
 
         //Add a XmlMap by a xml file.
         xmlMapCollection.add("xml.xml");
 
         wb.save("twoXmlMaps.xlsx");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| url | java.lang.String | url/chemin d'un fichier xml/xsd. |

**Returns:**
int - index de l'objet [XmlMap](../../com.aspose.cells/xmlmap).
### clear() {#clear--}
```
public void clear()
```


Supprime tous les XmlMaps.

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
public XmlMap get(int index)
```


Obtient le xml map par l'index spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap) - The xml map
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

