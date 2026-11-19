---
title: "HyperlinkCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.cells/hyperlinkcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HyperlinkCollection extends CollectionBase
```

Encapsule une collection d'objets [Hyperlink](../../com.aspose.cells/hyperlink).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Get Hyperlinks Collection
         HyperlinkCollection hyperlinks = worksheet.getHyperlinks();
 
         //Adding a hyperlink to a URL at "A1" cell
         hyperlinks.add("A1", 1, 1, "http://www.aspose.com");
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules. |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules. |
| [clear()](#clear--) | Efface tous les hyperliens. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [Hyperlink](../../com.aspose.cells/hyperlink) à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'hyperlien à l'index spécifié dans cette collection. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook();
         Worksheet worksheet = excel.getWorksheets().get(0);
         worksheet.getHyperlinks().add("A4", 1, 1, "http://www.aspose.com");
         worksheet.getHyperlinks().add("A5", 1, 1, "c:\\book1.xls");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Première ligne de la plage d'hyperliens. |
| firstColumn | int | Première colonne de la plage d'hyperliens. |
| totalRows | int | Nombre de lignes dans cette plage d'hyperliens. |
| totalColumns | int | Nombre de colonnes de cette plage d'hyperliens. |
| adresse | java.lang.String | Adresse du lien hypertexte. |

**Returns:**
int - index de l'objet [Hyperlink](../../com.aspose.cells/hyperlink).
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
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de cellule. |
| totalRows | int | Nombre de lignes dans cette plage d'hyperliens. |
| totalColumns | int | Nombre de colonnes de cette plage d'hyperliens. |
| adresse | java.lang.String | Adresse du lien hypertexte. |

**Returns:**
int - index de l'objet [Hyperlink](../../com.aspose.cells/hyperlink).
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startCellName | java.lang.String | La cellule en haut à gauche de la plage. |
| endCellName | java.lang.String | La cellule en bas à droite de la plage. |
| adresse | java.lang.String | Adresse du lien hypertexte. |
| textToDisplay | java.lang.String | Le texte à afficher pour le lien hypertexte spécifié. |
| screenTip | java.lang.String | Le texte d’infobulle pour le lien hypertexte spécifié. |

**Returns:**
int - index de l'objet [Hyperlink](../../com.aspose.cells/hyperlink).
### clear() {#clear--}
```
public void clear()
```


Efface tous les hyperliens.

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
public Hyperlink get(int index)
```


Obtient l'élément [Hyperlink](../../com.aspose.cells/hyperlink) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - The element at the specified index.
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


Supprime l'hyperlien à l'index spécifié dans cette collection.

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

