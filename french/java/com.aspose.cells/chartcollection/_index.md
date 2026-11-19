---
title: "ChartCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.cells/chartcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ChartCollection extends CollectionBase
```

Encapsule une collection d'objets [Chart](../../com.aspose.cells/chart).

**Example**

```
         Workbook workbook = new Workbook();
 
         ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-byte---java.lang.String-boolean-int-int-int-int-) | Ajoute un graphique avec un modèle prédéfini. |
| [add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)](#add-int-int-int-int-int-) | Ajoute un graphique à la collection. |
| [add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-boolean-int-int-int-int-) | Ajoute un graphique à la collection. |
| [add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-int-int-int-int-) | Ajoute un graphique à la collection. |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [addFloatingChart(int type, int left, int top, int width, int height)](#addFloatingChart-int-int-int-int-int-) | Ajoute un graphique à la collection. |
| [clear()](#clear--) | Efface tous les graphiques. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [Chart](../../com.aspose.cells/chart) à l'index spécifié. |
| [get(String name)](#get-java.lang.String-) | Obtient le graphique par son nom. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Chart chart)](#remove-com.aspose.cells.Chart-) | Supprime le graphique spécifique. |
| [removeAt(int index)](#removeAt-int-) | Supprime un graphique à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-byte---java.lang.String-boolean-int-int-int-int-}
```
public int add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Ajoute un graphique avec un modèle prédéfini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| données | byte[] | Les données du fichier de modèle de graphique (.crtx). |
| dataRange | java.lang.String | Spécifie la plage de données du graphique |
| isVertical | boolean | Spécifie si la série doit être tracée à partir d'une plage de valeurs de cellules par ligne ou par colonne. |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| rightRow | int | Indice de ligne en bas à droite |
| bottomColumn | int | Indice de colonne en bas à droite |

**Returns:**
int - index de l'objet [Chart](../../com.aspose.cells/chart).
### add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn) {#add-int-int-int-int-int-}
```
public int add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Ajoute un graphique à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Type de graphique |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| bottomRow | int | Indice de ligne en bas à droite |
| rightColumn | int | Indice de colonne en bas à droite |

**Returns:**
int - index de l'objet [Chart](../../com.aspose.cells/chart).
### add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-boolean-int-int-int-int-}
```
public int add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Ajoute un graphique à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Type de graphique |
| dataRange | java.lang.String | Spécifie la plage de données du graphique |
| isVertical | boolean | Spécifie si la série doit être tracée à partir d'une plage de valeurs de cellules par ligne ou par colonne. |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| rightRow | int | Indice de ligne en bas à droite |
| bottomColumn | int | Indice de colonne en bas à droite |

**Returns:**
int - index de l'objet [Chart](../../com.aspose.cells/chart).
### add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-int-int-int-int-}
```
public int add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Ajoute un graphique à la collection.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [add(int,String,boolean,int,int,int,int)](../../com.aspose.cells/chartcollection\#add-int-String-boolean-int-int-int-int-). Cette propriété sera supprimée 12 mois plus tard, depuis mai 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Type de graphique |
| dataRange | java.lang.String | Spécifie la plage de données du graphique |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| rightRow | int | Indice de ligne en bas à droite |
| bottomColumn | int | Indice de colonne en bas à droite |

**Returns:**
int - index de l'objet [Chart](../../com.aspose.cells/chart).
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
### addFloatingChart(int type, int left, int top, int width, int height) {#addFloatingChart-int-int-int-int-int-}
```
public int addFloatingChart(int type, int left, int top, int width, int height)
```


Ajoute un graphique à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Type de graphique |
| gauche | int | Le décalage x vers le coin |
| haut | int | Le décalage y vers le coin |
| largeur | int | La largeur du graphique |
| hauteur | int | La hauteur du graphique |

**Returns:**
int - index de l'objet [Chart](../../com.aspose.cells/chart).
### clear() {#clear--}
```
public void clear()
```


Efface tous les graphiques.

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
public Chart get(int index)
```


Obtient l'élément [Chart](../../com.aspose.cells/chart) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public Chart get(String name)
```


Obtient le graphique par son nom.

**Remarks**

Le nom par défaut du graphique est nul. Vous devez donc définir explicitement le nom du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom du graphique. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The chart.
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




### remove(Chart chart) {#remove-com.aspose.cells.Chart-}
```
public void remove(Chart chart)
```


Supprime le graphique spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chart | [Chart](../../com.aspose.cells/chart) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime un graphique à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index du graphique. |

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

