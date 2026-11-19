---
title: "PictureCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.cells/picturecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PictureCollection extends CollectionBase
```

Encapsule une collection d'objets [Picture](../../com.aspose.cells/picture).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //get PictureCollection
         PictureCollection pictures = workbook.getWorksheets().get(0).getPictures();
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#add-int-int-int-int-java.io.InputStream-) | Ajoute une image à la collection. |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | Ajoute une image à la collection. |
| [add(int topRow, int leftColumn, InputStream stream)](#add-int-int-java.io.InputStream-) | Ajoute une image à la collection. |
| [add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#add-int-int-java.io.InputStream-int-int-) | Ajoute une image à la collection. |
| [add(int topRow, int leftColumn, String fileName)](#add-int-int-java.lang.String-) | Ajoute une image à la collection. |
| [add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | Ajoute une image à la collection. |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [camera(int row, int column, String range)](#camera-int-int-java.lang.String-) | Prend une photo de la plage. |
| [clear()](#clear--) | Efface toutes les images. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [Picture](../../com.aspose.cells/picture) à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime les formes à l'index spécifié |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#add-int-int-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Ajoute une image à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| bottomRow | int | Indice de ligne en bas à droite |
| rightColumn | int | Indice de colonne en bas à droite |
| stream | java.io.InputStream | Objet de flux contenant les données de l'image. |

**Returns:**
int - index de l'objet [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)
```


Ajoute une image à la collection.

**Example**

```
         //add a picture
         pictures.add(1, 1, 5, 5, "image.jpg");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| bottomRow | int | Indice de ligne en bas à droite |
| rightColumn | int | Indice de colonne en bas à droite |
| fileName | java.lang.String | Nom de fichier de l'image. |

**Returns:**
int - index de l'objet [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, InputStream stream) {#add-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, InputStream stream)
```


Ajoute une image à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| stream | java.io.InputStream | Objet de flux contenant les données de l'image. |

**Returns:**
int - index de l'objet [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#add-int-int-java.io.InputStream-int-int-}
```
public int add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Ajoute une image à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| stream | java.io.InputStream | Objet de flux contenant les données de l'image. |
| widthScale | int | Échelle de la largeur de l'image, en pourcentage. |
| heightScale | int | Échelle de la hauteur de l'image, en pourcentage. |

**Returns:**
int - index de l'objet [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, String fileName)
```


Ajoute une image à la collection.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| fileName | java.lang.String | Nom de fichier de l'image. |

**Returns:**
int - index de l'objet [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)
```


Ajoute une image à la collection.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg", 50, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| fileName | java.lang.String | Nom de fichier de l'image. |
| widthScale | int | Échelle de la largeur de l'image, en pourcentage. |
| heightScale | int | Échelle de la hauteur de l'image, en pourcentage. |

**Returns:**
int - index de l'objet [Picture](../../com.aspose.cells/picture).
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
### camera(int row, int column, String range) {#camera-int-int-java.lang.String-}
```
public int camera(int row, int column, String range)
```


Prend une photo de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne de cette image. |
| colonne | int | L'index de colonne de cette image. |
| plage | java.lang.String | La zone qui nécessite une photographie |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


Efface toutes les images.

**Example**

```
         //clear
         pictures.clear();
```

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
public Picture get(int index)
```


Obtient l'élément [Picture](../../com.aspose.cells/picture) à l'index spécifié.

**Example**

```
         //get picture collection
         //PictureCollection pictures = workbook.Worksheets[0].Pictures;
         //add a picture
         int index = pictures.add(1, 1, "image.png");
         //get the picture
         Picture pic = pictures.get(index);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - The element at the specified index.
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


Supprime les formes à l'index spécifié

**Example**

```
         //add a picture
         int index2 = pictures.add(1, 1, "image.png");
         //delete
         pictures.removeAt(index2);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

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

