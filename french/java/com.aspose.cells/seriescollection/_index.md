---
title: "SeriesCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.cells/seriescollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```

Encapsule une collection d'objets [Series](../../com.aspose.cells/series).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String dataArea, boolean isVertical)](#add-java.lang.String-boolean-) | Ajoute la collection [Series](../../com.aspose.cells/series) à un graphique. |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | Ajoute la collection [Series](../../com.aspose.cells/series) à un graphique. |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | Ajoute la collection [Series](../../com.aspose.cells/series) à un graphique. |
| [changeColors(int type)](#changeColors-int-) | Définit la palette monochromatique pour les séries du graphique. |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | Modifie directement l'ordre des deux séries. |
| [clear()](#clear--) | Efface la collection |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [Series](../../com.aspose.cells/series) à l'index spécifié. |
| [getCategoryData()](#getCategoryData--) | Obtient la plage des valeurs de l'axe de catégorie. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [getSecondCategoryData()](#getSecondCategoryData--) | Obtient la plage des valeurs du deuxième axe de catégorie. |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | Obtient l'élément [Series](../../com.aspose.cells/series) par ordre. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [isColorVaried()](#isColorVaried--) | Indique si la couleur des points varie. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime une série à l'index spécifié. |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | Définit la plage des valeurs de l'axe de catégorie. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Indique si la couleur des points varie. |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | Définit la plage des valeurs du deuxième axe de catégorie. |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | Définit les noms de toutes les séries du graphique. |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | Modifie directement l'ordre des deux séries. |
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
### add(String dataArea, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String dataArea, boolean isVertical)
```


Ajoute la collection [Series](../../com.aspose.cells/series) à un graphique.

**Remarks**


Si les données sont définies sur des cellules contiguës, utilisez deux-points pour les séparer.Par exemple, $C$2:$C$5.

Si les données sont définies sur des cellules non contiguës, utilisez une virgule pour les séparer.Par exemple : ($C$2,$D$5).

Cette méthode ne fait qu'un simple traitement en tant que plage de données. Si vous souhaitez vérifier intelligemment la méthode ChartCollection.Add().


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dataArea | java.lang.String | Spécifie les valeurs à partir desquelles tracer la série de données |
| isVertical | boolean | Spécifie si la série doit être tracée à partir d'une plage de valeurs de cellules par ligne ou par colonne. Si vrai, [Series](../../com.aspose.cells/series) sera ajouté colonne par colonne |

**Returns:**
int - Retourne le premier indice de l'ASeries ajouté dans le NSeries.
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```


Ajoute la collection [Series](../../com.aspose.cells/series) à un graphique.

**Remarks**


Si les données sont définies sur des cellules contiguës, utilisez deux-points pour les séparer. Par exemple, $C$2:$C$5.

Si les données sont définies sur des cellules non contiguës, utilisez une virgule pour les séparer. Par exemple, ($C$2,$D$5).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| area | java.lang.String | Spécifie les valeurs à partir desquelles tracer la série de données |
| isVertical | boolean | Spécifie si la série doit être tracée à partir d'une plage de valeurs de cellules par ligne ou par colonne. |
| checkLabels | boolean | Indique si la plage contient le nom de la série |

**Returns:**
int - Retourne le premier indice de l'ASeries ajouté dans le NSeries.
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```


Ajoute la collection [Series](../../com.aspose.cells/series) à un graphique.

**Remarks**


Si les données sont définies sur des cellules contiguës, utilisez deux-points pour les séparer. Par exemple, R[1]C[1]:R[3]C[2].

Si les données sont définies sur des cellules contiguës, utilisez une virgule pour les séparer. Par exemple,(R[1]C[1],R[3]C[2]).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| area | java.lang.String | Spécifie les valeurs à partir desquelles tracer la série de données |
| isVertical | boolean | Spécifie si la série doit être tracée à partir d'une plage de valeurs de cellules par ligne ou par colonne. |

**Returns:**
int - Retourne le premier indice de l'ASeries ajouté dans le NSeries.
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```


Définit la palette monochromatique pour les séries du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype). Le type monochromatique. |

### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```


Modifie directement l'ordre des deux séries.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode SeriesCollection.SwapSeries. Cette méthode sera supprimée 12 mois plus tard, depuis juin 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceIndex | int | L'index actuel |
| destIndex | int | L'index de destination |

### clear() {#clear--}
```
public void clear()
```


Efface la collection

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
public Series get(int index)
```


Obtient l'élément [Series](../../com.aspose.cells/series) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```


Obtient la plage des valeurs de l'axe des catégories. Cela peut être une plage de cellules (par exemple "d1:e10") ou une séquence de valeurs (par exemple "\{2,6,8,10\}").

**Returns:**
java.lang.String
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
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```


Obtient la plage des valeurs du deuxième axe des catégories. Cela peut être une plage de cellules (par exemple, "d1:e10"), ou une séquence de valeurs (par exemple,"\{2,6,8,10\}"). N'affecte que lorsque certaines séries sont tracées sur le deuxième axe.

**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```


Obtient l'élément [Series](../../com.aspose.cells/series) par ordre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| order | int | L'ordre des séries |

**Returns:**
[Series](../../com.aspose.cells/series) - The element series
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
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Indique si la couleur des points varie.

**Remarks**

Fonctionne uniquement pour les graphiques circulaires ou lorsqu'il n'y a qu'une seule série.

**Returns:**
boolean
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


Supprime une série à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```


Définit la plage des valeurs de l'axe des catégories. Cela peut être une plage de cellules (par exemple "d1:e10") ou une séquence de valeurs (par exemple "\{2,6,8,10\}").

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Indique si la couleur des points varie.

**Remarks**

Fonctionne uniquement pour les graphiques circulaires ou lorsqu'il n'y a qu'une seule série.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```


Définit la plage des valeurs du deuxième axe des catégories. Cela peut être une plage de cellules (par exemple, "d1:e10"), ou une séquence de valeurs (par exemple,"\{2,6,8,10\}"). N'affecte que lorsque certaines séries sont tracées sur le deuxième axe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```


Définit les noms de toutes les séries du graphique.

**Remarks**


Si l'index de départ est supérieur au nombre de séries, la fonction retournera et ne fera rien.

Si les données sont définies sur des cellules contiguës, utilisez deux-points pour les séparer. Par exemple, $C$2:$C$5.

Si les données sont définies sur des cellules contiguës, utilisez une virgule pour les séparer. Par exemple, ($C$2,$D$5).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index de la première série dont vous souhaitez définir le nom. |
| area | java.lang.String | Spécifie la zone pour le nom de la série. |
| isVertical | boolean | >Spécifie si la série doit être tracée à partir d'une plage de valeurs de cellules par ligne ou par colonne. |

### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```


Modifie directement l'ordre des deux séries.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceIndex | int | L'index actuel |
| destIndex | int | L'index de destination |

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

