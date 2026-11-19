---
title: "ColumnCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Collection des objets qui représentent les paramètres de colonne individuels dans une feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/columncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ColumnCollection extends CollectionBase
```

Collection des objets [Column](../../com.aspose.cells/column) qui représentent les paramètres individuels de colonne dans une feuille de calcul. L'objet Column ne représente que les paramètres tels que la largeur de colonne, les styles, etc. pour toute la colonne, et n'a rien à voir avec la présence ou non de cellules non vides (données) dans la colonne correspondante. De plus, le \"Count\" de cette collection ne représente que le nombre d'objets Column qui ont été instanciés dans cette collection, et n'a rien à voir avec la présence ou non de cellules non vides (données) dans la feuille de calcul.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Add new Style to Workbook
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setForegroundColor(Color.getBlue());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.SOLID);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Change the default width of first ten columns
         for (int i = 0; i ? i++)
         {
             worksheet.getCells().getColumns().get(i).setWidth(20);
         }
 
         //Get the Column with non default formatting
         ColumnCollection columns = worksheet.getCells().getColumns();
 
         for (Column column : (Iterable<Column>) columns)
         {
             //Apply Style to first ten Columns
             column.applyStyle(style, styleFlag);
         }
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int columnIndex)](#get-int-) | Obtient un objet [Column](../../com.aspose.cells/column) par indice de colonne. |
| [getByIndex(int index)](#getByIndex-int-) | Obtient l'objet colonne par l'index. |
| [getClass()](#getClass--) |  |
| [getColumnByIndex(int index)](#getColumnByIndex-int-) | Obtient l'objet [Column](../../com.aspose.cells/column) par la position dans la liste. |
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
### get(int columnIndex) {#get-int-}
```
public Column get(int columnIndex)
```


Obtient un objet [Column](../../com.aspose.cells/column) par l'index de colonne. L'objet Column de l'index de colonne donné sera instancié s'il n'existe pas auparavant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int |  |

**Returns:**
[Column](../../com.aspose.cells/column)
### getByIndex(int index) {#getByIndex-int-}
```
public Column getByIndex(int index)
```


Obtient l'objet colonne par l'index.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Columns.GetColumnByIndex(). Cette propriété sera supprimée 12 mois plus tard à compter de juin 2010. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnByIndex(int index) {#getColumnByIndex-int-}
```
public Column getColumnByIndex(int index)
```


Obtient l'objet [Column](../../com.aspose.cells/column) par la position dans la liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | La position dans la liste. |

**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
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

