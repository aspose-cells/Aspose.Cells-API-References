---
title: "GridPivotTableCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.gridweb/gridpivottablecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```

Encapsule une collection d'objets [GridPivotTable](../../com.aspose.gridweb/gridpivottable).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Ajoute un nouveau cache de PivotTable à une collection PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | Ajoute un nouveau cache de PivotTable à une collection PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Ajoute un nouveau cache de PivotTable à une collection PivotCaches. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Ajoute un nouveau cache de PivotTable à une collection PivotCaches. |
| [clear()](#clear--) | Efface toutes les PivotTables. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [GridPivotTable](../../com.aspose.gridweb/gridpivottable) à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient la taille de l'énumérateur |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime la PivotTable à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```


Ajoute un nouveau cache de PivotTable à une collection PivotCaches.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | La feuille de calcul source. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | La zone dans la feuille de calcul source. |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice du nouveau cache ajouté.
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```


Ajoute un nouveau cache de PivotTable à une collection PivotCaches.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| worksheetname | java.lang.String | Le nom de la feuille de calcul source. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | La zone dans la feuille de calcul source. |
| destRow | int | La ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport PivotTable. |
| destCol | int | La colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport PivotTable. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice du nouveau cache ajouté.
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```


Ajoute un nouveau cache de PivotTable à une collection PivotCaches.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| worksheetname | java.lang.String | Le nom de la feuille de calcul source. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | La zone dans la feuille de calcul source. |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice du nouveau cache ajouté.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Ajoute un nouveau cache de PivotTable à une collection PivotCaches.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | La plage de cellules de données pour le nouveau tableau croisé dynamique.Exemple : Sheet1!A1:C8 |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice du nouveau cache ajouté.
### clear() {#clear--}
```
public void clear()
```


Efface toutes les PivotTables.

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
public GridPivotTable get(int index)
```


Obtient l'élément [GridPivotTable](../../com.aspose.gridweb/gridpivottable) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[GridPivotTable](../../com.aspose.gridweb/gridpivottable) - The element at the specified index.
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


Obtient la taille de l'énumérateur

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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


Supprime la PivotTable à l'index spécifié.

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

