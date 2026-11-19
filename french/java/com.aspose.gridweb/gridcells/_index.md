---
title: "GridCells"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.gridweb/gridcells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```

Encapsule une collection d'objets [GridCell](../../com.aspose.gridweb/gridcell).
## Méthodes

| Méthode | Description |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Obtient le nom de la cellule selon ses indices de ligne et de colonne. |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | Obtient les index de ligne et de colonne de la cellule selon son nom |
| [checkCell(int row, int column)](#checkCell-int-int-) | Obtient l'élément [GridCell](../../com.aspose.gridweb/gridcell) ou null à l'index de ligne et de colonne de cellule spécifié. |
| [checkColumn(int col)](#checkColumn-int-) | Obtient l'élément [GridColumn](../../com.aspose.gridweb/gridcolumn) ou null à l'index de colonne spécifié. |
| [checkRow(int i)](#checkRow-int-) | Obtient l'élément [GridRow](../../com.aspose.gridweb/gridrow) ou null à l'index de ligne de cellule spécifié. |
| [clear()](#clear--) | Efface toutes les cellules de la collection. |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | Efface le contenu d'une plage. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Efface le contenu d'une plage. |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | Efface le formatage d'une plage. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Efface le formatage d'une plage. |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | Efface le contenu et le formatage d'une plage. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Efface le contenu et le formatage d'une plage. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Obtient le nom de la colonne selon l'indice de colonne. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Obtient l'indice de colonne selon le nom de la colonne. |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | Copie les données et le formatage d'une colonne entière. |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | Copie les données et le formatage d'une colonne entière. |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | Copie les données et le formatage d'une ligne entière. |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | Copie les données et le formatage de plusieurs lignes entières. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Supprime toutes les colonnes vides qui ne contiennent aucune donnée. |
| [deleteBlankRows()](#deleteBlankRows--) | Supprime toutes les lignes vides qui ne contiennent aucune donnée. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Supprime une colonne. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Supprime une colonne. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Supprime plusieurs colonnes. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Supprime une plage de cellules et décale les cellules selon l'option de décalage. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Supprime une ligne. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Supprime plusieurs lignes. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Supprime plusieurs lignes dans la feuille de calcul. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exporte les données de la collection [GridCells](../../com.aspose.gridweb/gridcells) vers un objet tableau à deux dimensions. |
| [get(int row, int column)](#get-int-int-) | Obtient l'élément [GridCell](../../com.aspose.gridweb/gridcell) à l'index de ligne et de colonne de cellule spécifié. |
| [get(String cellName)](#get-java.lang.String-) | Obtient l'élément [GridCell](../../com.aspose.gridweb/gridcell) au nom de cellule spécifié. |
| [getCell(int row, int column)](#getCell-int-int-) | Obtient l'élément [GridCell](../../com.aspose.gridweb/gridcell) à l'index de ligne et de colonne de cellule spécifié. |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Obtient la largeur de la colonne spécifiée |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Obtient la largeur de la colonne spécifiée, en pouces. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Obtient la largeur de la colonne spécifiée, en pixels. |
| [getColumns()](#getColumns--) | Obtient la collection d'objets [GridColumn](../../com.aspose.gridweb/gridcolumn) qui représente les colonnes individuelles de cette feuille de calcul. |
| [getCount()](#getCount--) | Obtient le nombre de cellules. |
| [getFirstCell()](#getFirstCell--) | Récupère la première cellule de cette feuille de calcul. |
| [getLastCell()](#getLastCell--) | Récupère la dernière cellule de cette feuille de calcul. |
| [getMaxColumn()](#getMaxColumn--) | Index de colonne maximal de la cellule qui contient des données ou un style. |
| [getMaxDataColumn()](#getMaxDataColumn--) | Indice maximal de colonne de la cellule qui contient des données. |
| [getMaxDataRow()](#getMaxDataRow--) | Indice maximal de ligne de la cellule qui contient des données. |
| [getMaxRow()](#getMaxRow--) | Indice maximal de ligne de la cellule qui contient des données ou un style. |
| [getMergedCells()](#getMergedCells--) | Obtient la collection des cellules fusionnées. |
| [getMinColumn()](#getMinColumn--) | Indice de colonne minimum de ces cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée). |
| [getMinDataColumn()](#getMinDataColumn--) | Indice de colonne minimum de la cellule qui contient des données. |
| [getMinDataRow()](#getMinDataRow--) | Indice de ligne minimum de la cellule qui contient des données. |
| [getMinRow()](#getMinRow--) | Indice de ligne minimum de la cellule qui contient des données ou un style. |
| [getRow(int i)](#getRow-int-) | Obtient l'élément [GridRow](../../com.aspose.gridweb/gridrow) ou à l'index de ligne de cellule spécifié. |
| [getRowEnumerator()](#getRowEnumerator--) | Obtient l'énumérateur des lignes |
| [getRowHeight(int row)](#getRowHeight-int-) | Obtient la hauteur d'une ligne spécifiée. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Obtient la hauteur d'une ligne spécifiée en pixels. |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | Obtient le niveau de contour de la ligne. |
| [getRows()](#getRows--) | Obtient la collection d'objets [GridRow](../../com.aspose.gridweb/gridrow) qui représente les lignes individuelles de cette feuille de calcul. |
| [getStandardHeight()](#getStandardHeight--) | Obtient la hauteur de ligne par défaut dans cette feuille, en points. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Obtient la hauteur de ligne par défaut dans cette feuille, en pixels. |
| [getStandardWidth()](#getStandardWidth--) | Obtient la largeur de colonne par défaut dans la feuille de calcul, en unités de caractères. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Obtient la largeur de colonne par défaut dans la feuille de calcul, en pouces. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Obtient la largeur de colonne par défaut dans la feuille de calcul, en pixels. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Obtenez la largeur dans différents types de vue. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Regroupe les colonnes. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Regroupe les colonnes. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Regroupe les lignes. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Masque une colonne. |
| [hideRow(int row)](#hideRow-int-) | Masque une ligne. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Insère une nouvelle colonne dans la feuille de calcul. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Insère une nouvelle colonne dans la feuille de calcul. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Insère plusieurs colonnes dans la feuille de calcul. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Insère plusieurs colonnes dans la feuille de calcul. |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [insertRow(int rowIndex)](#insertRow-int-) | Insère une nouvelle ligne dans la feuille de calcul. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Insère plusieurs lignes dans la feuille de calcul. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Insère plusieurs lignes dans la feuille de calcul. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Vérifie si la colonne donnée est vide (ne contient aucune donnée). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Vérifie si une colonne à l'index donné est masquée. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Vérifie si une ligne à l'index donné est masquée. |
| [iterator()](#iterator--) | Obtient l'énumérateur des lignes |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | Déplace la plage. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Supprime les valeurs dupliquées dans la plage. |
| [removeFormulas()](#removeFormulas--) | Supprime toutes les formules et les remplace par la valeur de la formule. |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | Définit les bordures pour une plage de cellules. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Définit la largeur de la colonne spécifiée. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Définit la largeur de colonne en unités de pouces. |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | Définit la largeur de colonne en unités de pixels. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Définit la hauteur de la ligne spécifiée. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Définit la hauteur de la ligne en unités de pouces. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Définit la hauteur de la ligne en unités de pixels. |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | Définit le niveau de contour de la ligne. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Définit la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Définit la largeur de colonne par défaut dans la feuille de calcul, en unités de caractères. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Définit la largeur de colonne par défaut dans la feuille de calcul, en unités de pouces. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Définit la largeur de colonne par défaut dans la feuille de calcul, en unités de pixels. |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | Applique le style à une plage de cellules spécifiée. |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | Applique le style à une plage de cellules spécifiée. |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | Trie les données en ordre ascendant/descendant de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | Trie les données en ordre ascendant/descendant de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Annule la fusion d’une plage spécifiée de cellules fusionnées. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Dégroupe les colonnes. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Dégroupe les lignes. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Affiche une colonne |
| [unhideRow(int row)](#unhideRow-int-) | Affiche une ligne. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Obtient le nom de la cellule selon ses indices de ligne et de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| colonne | int | Indice de colonne. |

**Returns:**
java.lang.String - Nom de la cellule.
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```


Obtient les index de ligne et de colonne de la cellule selon son nom

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de la cellule. |
| ligne | int | Indice de ligne de sortie |
| colonne | int | Indice de colonne de sortie |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```


Obtient l'élément [GridCell](../../com.aspose.gridweb/gridcell) ou null à l'index de ligne et de colonne de cellule spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne |
| colonne | int | Indice de colonne |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```


Obtient l'élément [GridColumn](../../com.aspose.gridweb/gridcolumn) ou null à l'index de colonne spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| col | int | L'index de colonne. |

**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```


Obtient l'élément [GridRow](../../com.aspose.gridweb/gridrow) ou null à l'index de ligne de cellule spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| i | int | Indice de ligne |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Efface toutes les cellules de la collection.

### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```


Efface le contenu d'une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Plage à effacer. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Efface le contenu d'une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| startColumn | int | Indice de colonne de départ. |
| endRow | int | Indice de ligne de fin. |
| endColumn | int | Indice de colonne de fin. |

### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```


Efface le formatage d'une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Plage à effacer. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Efface le formatage d'une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| startColumn | int | Indice de colonne de départ. |
| endRow | int | Indice de ligne de fin. |
| endColumn | int | Indice de colonne de fin. |

### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```


Efface le contenu et le formatage d'une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Plage à effacer. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Efface le contenu et le formatage d'une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| startColumn | int | Indice de colonne de départ. |
| endRow | int | Indice de ligne de fin. |
| endColumn | int | Indice de colonne de fin. |

### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Obtient le nom de la colonne selon l'indice de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |

**Returns:**
java.lang.String - Nom de la colonne.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Obtient l'indice de colonne selon le nom de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnName | java.lang.String | Nom de la colonne. |

**Returns:**
int - Indice de colonne.
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Copie les données et le formatage d'une colonne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | L'objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | int | Indice de colonne source. |
| destinationColumnIndex | int | Indice de colonne de destination. |

### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Copie les données et le formatage d'une colonne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | L'objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | int | Indice de colonne source. |
| destinationColumnIndex | int | Indice de colonne de destination. |
| columnNumber | int | Le numéro de colonne copié. |

### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Copie les données et le formatage d'une ligne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | L'objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | int | Indice de ligne source. |
| destinationRowIndex | int | Indice de ligne de destination. |

### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Copie les données et le formatage de plusieurs lignes entières.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | L'objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | int | Indice de ligne source. |
| destinationRowIndex | int | Indice de ligne de destination. |
| rowNumber | int | Le numéro de ligne copié. |

### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Supprime toutes les colonnes vides qui ne contiennent aucune donnée.

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Supprime toutes les lignes vides qui ne contiennent aucune donnée.

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Supprime une colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Supprime une colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |
| updateReference | boolean | Indique s'il faut mettre à jour les références dans les autres feuilles de calcul. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Supprime plusieurs colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |
| totalColumns | int | Nombre de colonnes à supprimer. |
| updateReference | boolean | Indique s'il faut mettre à jour les références dans les autres feuilles de calcul. |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Supprime une plage de cellules et décale les cellules selon l'option de décalage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| startColumn | int | Indice de colonne de départ. |
| endRow | int | Indice de ligne de fin. |
| endColumn | int | Indice de colonne de fin. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Option de déplacement des cellules. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Supprime une ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de ligne. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Supprime plusieurs lignes.

**Remarks**

Si la plage supprimée contient la partie supérieure (pas la totalité) du tableau (ListObject), la plage ne peut pas être supprimée et aucune action ne sera effectuée. Cela fonctionne comme MS Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de la première ligne à supprimer. |
| totalRows | int | Nombre de lignes à supprimer. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Supprime plusieurs lignes dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de ligne. |
| totalRows | int | Nombre de lignes à supprimer. |
| updateReference | boolean | Indique s'il faut mettre à jour les références dans les autres feuilles de calcul. |

**Returns:**
boolean -
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
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exporte les données de la collection [GridCells](../../com.aspose.gridweb/gridcells) vers un objet tableau à deux dimensions.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Numéro de ligne de la première cellule à exporter. |
| firstColumn | int | Numéro de colonne de la première cellule à exporter |
| totalRows | int | Nombre de lignes à exporter |
| totalColumns | int | Nombre de colonnes à exporter |

**Returns:**
java.lang.Object[][] - Objet tableau de valeurs de cellules exportées.
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```


Obtient l'élément [GridCell](../../com.aspose.gridweb/gridcell) à l'index de ligne et de colonne de cellule spécifié.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
         //Gets the cell at "A1"
         GridCell cell = cells.get(0, 0);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| colonne | int | Indice de colonne. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```


Obtient l'élément [GridCell](../../com.aspose.gridweb/gridcell) au nom de cellule spécifié.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
          GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
          GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de la cellule, incluant sa lettre de colonne et son numéro de ligne, par exemple A5. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```


Obtient l'élément [GridCell](../../com.aspose.gridweb/gridcell) à l'index de ligne et de colonne de cellule spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne |
| colonne | int | Indice de colonne |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return Cell object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Obtient la largeur de la colonne spécifiée

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne |

**Returns:**
double - Largeur de la colonne
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Obtient la largeur de la colonne spécifiée, en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne |

**Returns:**
double - Largeur de la colonne
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Obtient la largeur de la colonne spécifiée, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne |

**Returns:**
int - Largeur de la colonne en vue normale.
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```


Obtient la collection d'objets [GridColumn](../../com.aspose.gridweb/gridcolumn) qui représente les colonnes individuelles de cette feuille de calcul.

**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre de cellules.

**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Récupère la première cellule de cette feuille de calcul.

**Remarks**

Renvoie null s'il n'y a aucune donnée dans la feuille de calcul.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Récupère la dernière cellule de cette feuille de calcul.

**Remarks**

Renvoie null s'il n'y a aucune donnée dans la feuille de calcul.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Index de colonne maximal de la cellule qui contient des données ou un style.

**Remarks**

Retourne -1 s'il n'y a pas de cellule.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Indice maximal de colonne de la cellule qui contient des données.

**Remarks**

\-1 sera retourné s'il n'y a aucune cellule contenant des données. Cette propriété doit parcourir et vérifier toutes les cellules d'une feuille de calcul, ce qui consomme du temps et ne doit pas être invoquée de manière répétée.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Indice maximal de ligne de la cellule qui contient des données.

**Remarks**

Retourne -1 s'il n'y a aucune cellule contenant des données.

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Indice maximal de ligne de la cellule qui contient des données ou un style.

**Remarks**

Retourne -1 s'il n'y a aucune cellule contenant des données ou un style dans la feuille de calcul.

**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Obtient la collection des cellules fusionnées.

**Remarks**

Dans cette collection, chaque élément est une structure [GridCellArea](../../com.aspose.gridweb/gridcellarea) qui représente une zone de cellules fusionnées.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Indice de colonne minimum de ces cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée).

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Indice de colonne minimum de la cellule qui contient des données.

**Remarks**

\-1 sera retourné s'il n'y a aucune cellule contenant des données. Cette propriété doit parcourir et vérifier toutes les cellules d'une feuille de calcul, ce qui consomme du temps et ne doit pas être invoquée de manière répétée.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Indice de ligne minimum de la cellule qui contient des données.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Indice de ligne minimum de la cellule qui contient des données ou un style.

**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```


Obtient l'élément [GridRow](../../com.aspose.gridweb/gridrow) ou à l'index de ligne de cellule spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| i | int | Indice de ligne |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Obtient l'énumérateur des lignes

**Returns:**
java.util.Iterator - L'énumérateur des lignes.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Obtient la hauteur d'une ligne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne |

**Returns:**
double - Hauteur de la ligne
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Obtient la hauteur d'une ligne spécifiée en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne |

**Returns:**
double - Hauteur de la ligne
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Obtient la hauteur d'une ligne spécifiée en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne |

**Returns:**
int - Hauteur de la ligne
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```


Obtient le niveau de contour de la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | indice de ligne. |

**Returns:**
int - le niveau de contour.
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```


Obtient la collection d'objets [GridRow](../../com.aspose.gridweb/gridrow) qui représente les lignes individuelles de cette feuille de calcul.

**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Obtient la hauteur de ligne par défaut dans cette feuille, en points.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Obtient la hauteur de ligne par défaut dans cette feuille, en pixels.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Obtient la largeur de colonne par défaut dans la feuille de calcul, en unités de caractères.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Obtient la largeur de colonne par défaut dans la feuille de calcul, en pouces.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Obtient la largeur de colonne par défaut dans la feuille de calcul, en pixels.

**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Obtenez la largeur dans différents types de vue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | L'index de colonne. |

**Returns:**
int - la largeur de la colonne en pixels
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Regroupe les colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de colonne à regrouper. |
| lastIndex | int | Le dernier indice de colonne à regrouper. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Regroupe les colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de colonne à regrouper. |
| lastIndex | int | Le dernier indice de colonne à regrouper. |
| isHidden | boolean | Spécifie si les colonnes regroupées sont masquées. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Regroupe les lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de ligne à regrouper. |
| lastIndex | int | Le dernier indice de ligne à regrouper. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


Masque une colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Masque une ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Insère une nouvelle colonne dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Insère une nouvelle colonne dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |
| updateReference | boolean | Indique si les références dans d’autres feuilles de calcul seront mises à jour. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Insère plusieurs colonnes dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |
| totalColumns | int | Le nombre de colonnes. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Insère plusieurs colonnes dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |
| totalColumns | int | Le nombre de colonnes. |
| updateReference | boolean | Indique si les références dans d’autres feuilles de calcul seront mises à jour. |

### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```


Insère une plage de cellules et décale les cellules selon l'option de décalage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Déplacer la zone. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Option de déplacement des cellules. |

### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Insère une plage de cellules et décale les cellules selon l'option de décalage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Déplacer la zone. |
| shiftNumber | int | Nombre de lignes ou de colonnes à insérer. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Option de déplacement des cellules. |
| updateReference | boolean | Indique s'il faut mettre à jour les références dans les autres feuilles de calcul. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Insère une nouvelle ligne dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de ligne. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Insère plusieurs lignes dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de ligne. |
| totalRows | int | Nombre de lignes à insérer. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Insère plusieurs lignes dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de ligne. |
| totalRows | int | Nombre de lignes à insérer. |
| updateReference | boolean | Indique si les références dans d’autres feuilles de calcul seront mises à jour. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Vérifie si la colonne donnée est vide (ne contient aucune donnée).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | l'index de colonne |

**Returns:**
booléen - vrai si la colonne donnée ne contient aucune donnée
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Vérifie si une colonne à l'index donné est masquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | index de colonne |

**Returns:**
booléen - vrai si la colonne est masquée.
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Vérifie si une ligne à l'index donné est masquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | indice de ligne |

**Returns:**
booléen - vrai si la ligne est masquée
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtient l'énumérateur des lignes

**Returns:**
java.util.Iterator - L'énumérateur des lignes
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Fusionne une plage de cellules spécifiée en une seule cellule.

**Remarks**

Référez la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Première ligne de cette plage (index zéro) |
| firstColumn | int | Première colonne de cette plage (index zéro) |
| totalRows | int | Nombre de lignes (index à partir de 1) |
| totalColumns | int | Nombre de colonnes (base 1) |

### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```


Déplace la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | La plage qui doit être déplacée. |
| destRow | int | La ligne de destination. |
| destColumn | int | La colonne de destination. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Supprime les valeurs dupliquées dans la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ. |
| startColumn | int | La colonne de départ |
| endRow | int | L'index de la ligne de fin. |
| endColumn | int | L'index de la colonne de fin. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Supprime toutes les formules et les remplace par la valeur de la formule.

### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```


Définit les bordures pour une plage de cellules.

**Example**

```
           GridWeb GridWeb1 = new GridWeb();
           WebBorderStyle borderStyle1 = new WebBorderStyle();
         	 GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Le numéro de la première ligne de la plage (indice zéro). |
| firstColumn | int | Le numéro de la première colonne de la plage (indice zéro). |
| rowNumber | int | Le nombre de lignes. |
| columnNumber | int | Le nombre de colonnes. |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition). La position de la bordure. |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Le style de la bordure. |

### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Définit la largeur de la colonne spécifiée.

**Remarks**

Pour masquer une colonne, définissez la largeur de la colonne à zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| largeur | double | Largeur de la colonne. La largeur de la colonne doit être comprise entre 0 et 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Définit la largeur de colonne en unités de pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| inches | double | Nombre de pouces. |

### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```


Définit la largeur de colonne en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| pixel | int | Nombre de pixels. |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Définit la hauteur de la ligne spécifiée.

**Remarks**

Pour masquer une ligne, définissez la hauteur de la ligne à zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| hauteur | double | Hauteur de la ligne. En unité de point, elle doit être comprise entre 0 et 409,5. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Définit la hauteur de la ligne en unités de pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| inches | double | Nombre de pouces. Il doit être compris entre 0 et 409,5/72. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Définit la hauteur de la ligne en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| pixels | int | Nombre de pixels. |

### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```


Définit le niveau de contour de la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | indice de ligne. |
| outlineLevel | int | niveau de contour. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Définit la hauteur de ligne par défaut dans cette feuille de calcul, en points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Définit la largeur de colonne par défaut dans la feuille de calcul, en unités de caractères.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Définit la largeur de colonne par défaut dans la feuille de calcul, en unités de pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Définit la largeur de colonne par défaut dans la feuille de calcul, en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```


Applique le style à une plage de cellules spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Première ligne de cette plage (index zéro) |
| firstColumn | int | Première colonne de cette plage (index zéro) |
| rowNumber | int | Nombre de lignes (index à partir de 1) |
| columnNumber | int | Nombre de colonnes (base 1) |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | L'objet de style à définir |

### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```


Applique le style à une plage de cellules spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellRange | java.lang.String | La plage des noms de cellules, comme "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | L'objet de style à définir |

### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```


Trie les données en ordre ascendant/descendant de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. Trie les données en ordre ascendant/descendant de gauche à droite dans une plage d'une feuille de calcul selon l'index de ligne spécifié.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Le numéro de ligne de la première cellule à trier. |
| startColumn | int | Le numéro de colonne de la première cellule à trier. |
| lignes | int | Nombre de lignes à importer. |
| colonnes | int | Nombre de colonnes à importer. |
| index | int | L'index de colonne qui spécifie la colonne de tri. Si l'Orientation est de haut en bas, il représente l'index de colonne qui spécifie la colonne de tri. Si l'Orientation est de gauche à droite, il représente l'index de ligne qui spécifie la ligne de tri. |
| isAsending | boolean | si l'ordre de tri est ascendant. |
| isCaseSensitive | boolean | si le tri est sensible à la casse. |
| islefttoright | boolean | si l'orientation du tri est de gauche à droite |

### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```


Trie les données en ordre ascendant/descendant de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. Trie les données en ordre ascendant/descendant de gauche à droite dans une plage d'une feuille de calcul selon l'index de ligne spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Le numéro de ligne de la première cellule à trier. |
| startColumn | int | Le numéro de colonne de la première cellule à trier. |
| lignes | int | Nombre de lignes à importer. |
| colonnes | int | Nombre de colonnes à importer. |
| indices | int[] | Le tableau d'index de colonne qui spécifie la colonne de tri. Si l'Orientation est de haut en bas, il représente l'index de colonne qui spécifie la colonne de tri. Si l'Orientation est de gauche à droite, il représente l'index de ligne qui spécifie la ligne de tri. |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder). le tableau d'ordre de tri. |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation). orientation du tri |
| isCaseSensitive | boolean | si le tri est sensible à la casse. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#unMerge-int-int-int-int-}
```
public void unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Annule la fusion d’une plage spécifiée de cellules fusionnées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Première ligne de cette plage (index zéro) |
| firstColumn | int | Première colonne de cette plage (index zéro) |
| totalRows | int | Nombre de lignes (index à partir de 1) |
| totalColumns | int | Nombre de colonnes (base 1) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Dégroupe les colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de colonne à dégrouper. |
| lastIndex | int | Le dernier indice de colonne à dégrouper. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Dégroupe les lignes.

**Remarks**

Supprime uniquement les informations du groupe externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de ligne à dégrouper. |
| lastIndex | int | Le dernier indice de ligne à dégrouper. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Affiche une colonne

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| largeur | double | Largeur de colonne..La largeur de colonne doit être comprise entre 0 et 255 |

### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```


Affiche une ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |

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

