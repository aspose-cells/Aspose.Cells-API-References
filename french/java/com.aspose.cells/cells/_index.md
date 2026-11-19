---
title: "Cells"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets pertinents pour les cellules tels que ...etc."
type: docs
url: /fr/java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

Encapsule une collection d'objets pertinents pour les cellules, tels que [Cell](../../com.aspose.cells/cell), [Row](../../com.aspose.cells/row), ...etc.

**Remarks**

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
 
         	//Set default row height
         	cells.setStandardHeight(20);
         	//Set row height
         	cells.setRowHeight(2, 20.5);
 
         	//Set default colum width
         	cells.setStandardWidth(15);
         	//Set column width
         	cells.setColumnWidth(3, 12.57);
 
         	//Merge cells
         	cells.merge(5, 4, 2, 2);
 
         	//Put values to cells
         	cells.get(0, 0).putValue(true);
         	cells.get(0, 1).putValue(1);
         	cells.get(0, 2).putValue("abc");
 
         //Export data
         Object[][] arr = cells.exportArray(0, 0, 10, 10);
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | Ajoute une référence d'objet de plage aux cellules |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applique des formats à une colonne entière. |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applique des formats à une ligne entière. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applique des formats à une feuille de calcul entière. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Obtient l'élément [Cell](../../com.aspose.cells/cell) ou null à l'indice de ligne et de colonne de cellule spécifié. |
| [checkColumn(int columnIndex)](#checkColumn-int-) | Obtient l'élément [Column](../../com.aspose.cells/column) ou null à l'indice de colonne spécifié. |
| [checkRow(int row)](#checkRow-int-) | Obtient l'élément [Row](../../com.aspose.cells/row) ou null à l'indice de ligne de cellule spécifié. |
| [clear()](#clear--) | Efface toutes les données de la feuille de calcul. |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | Efface le contenu d'une plage. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Efface le contenu d'une plage. |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | Efface le formatage d'une plage. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Efface le formatage d'une plage. |
| [clearMergedCells()](#clearMergedCells--) | Efface toutes les plages fusionnées. |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | Efface le contenu et le formatage d'une plage. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Efface le contenu et le formatage d'une plage. |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | Convertit toutes les données de type chaîne de la feuille de calcul en valeur numérique si possible. |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | Copie les données et les formats d'une colonne entière. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | Copie les données et les formats de colonnes entières. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | Copie les données et les formats d'une colonne entière. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | Copie les données et les formats de toutes les colonnes. |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | Copie les données et les formats d'une ligne entière. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | Copie les données et les formats de certaines lignes entières. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | Copie les données et les formats de certaines lignes entières. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | Copie les données et les formats de certaines lignes entières. |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | Crée un objet [Range](../../com.aspose.cells/range) à partir de lignes de cellules ou de colonnes de cellules. |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | Crée un objet [Range](../../com.aspose.cells/range) à partir d'une plage de cellules. |
| [createRange(String address)](#createRange-java.lang.String-) | Crée un objet [Range](../../com.aspose.cells/range) à partir d'une adresse de la plage. |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | Crée un objet [Range](../../com.aspose.cells/range) à partir d'une plage de cellules. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Supprime toutes les colonnes vides qui ne contiennent aucune donnée. |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | Supprime toutes les colonnes vides qui ne contiennent aucune donnée. |
| [deleteBlankRows()](#deleteBlankRows--) | Supprime toutes les lignes vides qui ne contiennent aucune donnée ou aucun autre objet. |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | Supprime toutes les lignes vides qui ne contiennent aucune donnée ou certains objets spéciaux tels que les commentaires visibles, les tableaux croisés dynamiques. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Supprime une colonne. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Supprime une colonne. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Supprime plusieurs colonnes. |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | Supprime plusieurs colonnes. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Supprime une plage de cellules et décale les cellules selon l'option de décalage. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Supprime une ligne. |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | Supprime une ligne. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Supprime plusieurs lignes. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Supprime plusieurs lignes dans la feuille de calcul. |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | Supprime plusieurs lignes dans la feuille de calcul. |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | Obtient la dernière cellule de cette colonne. |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | Obtient la dernière cellule avec l'index de colonne maximal dans cette plage. |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | Obtient la dernière cellule de cette ligne. |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | Obtient la dernière cellule avec l'index de ligne maximal dans cette plage. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exporte les données de la collection [Cells](../../com.aspose.cells/cells) vers un objet tableau à deux dimensions. |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | Exporte le type de valeur des cellules de la collection [Cells](../../com.aspose.cells/cells) vers un objet tableau à deux dimensions. |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | Trouve la cellule contenant l'objet d'entrée. |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | Trouve la cellule contenant l'objet d'entrée. |
| [get(int row, int column)](#get-int-int-) | Obtient l'élément [Cell](../../com.aspose.cells/cell) aux index de ligne et de colonne de cellule spécifiés. |
| [get(String cellName)](#get-java.lang.String-) | Obtient l'élément [Cell](../../com.aspose.cells/cell) au nom de cellule spécifié. |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | Obtient le style d'affichage de la cellule donnée. |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | Obtient le style d'affichage de la cellule donnée. |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | Obtenez le style de la cellule donnée. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | Récupère toutes les cellules qui contiennent une image intégrée. |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | Récupère la hauteur d'origine de la colonne en points si la colonne est masquée |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Récupère la largeur (en nombre de caractères) de la colonne spécifiée en vue normale |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | Récupère la largeur de la colonne. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Récupère la largeur de la colonne spécifiée en vue normale, en pouces. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Récupère la largeur de la colonne spécifiée en vue normale, en pixels. |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | Récupère la largeur de la colonne spécifiée en vue normale, en pixels. |
| [getColumns()](#getColumns--) | Récupère la collection d'objets [Column](../../com.aspose.cells/column) qui représente les colonnes individuelles dans cette feuille de calcul. |
| [getCount()](#getCount--) | Récupère le nombre total d'objets Cell instanciés. |
| [getCountLarge()](#getCountLarge--) | Récupère le nombre total d'objets Cell instanciés. |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | Obtenez toutes les cellules qui font référence à la cellule spécifique. |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | Récupère toutes les cellules dont le résultat calculé dépend de la cellule spécifique. |
| [getFirstCell()](#getFirstCell--) | Récupère la première cellule de cette feuille de calcul. |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | Récupère l'index de la première ligne de la cellule qui contient des données dans la colonne spécifiée. |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | Récupère le niveau de contour (à partir de zéro) de la colonne. |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | Récupère le niveau de contour (à partir de zéro) de la ligne. |
| [getLastCell()](#getLastCell--) | Récupère la dernière cellule de cette feuille de calcul. |
| [getLastDataRow(int column)](#getLastDataRow-int-) | Récupère l'index de la dernière ligne de la cellule qui contient des données dans la colonne spécifiée. |
| [getMaxColumn()](#getMaxColumn--) | Indice maximal de colonne des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée). |
| [getMaxDataColumn()](#getMaxDataColumn--) | Indice maximal de colonne de la cellule qui contient des données. |
| [getMaxDataRow()](#getMaxDataRow--) | Indice maximal de ligne de la cellule qui contient des données. |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | Récupère la plage maximale qui inclut les données, les cellules fusionnées et les formes. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | Récupère le niveau de contour maximal des colonnes groupées (à partir de zéro). |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | Récupère le niveau de contour maximal des lignes groupées (à partir de zéro). |
| [getMaxRow()](#getMaxRow--) | Indice maximal de ligne de la cellule qui contient des données ou un style. |
| [getMemorySetting()](#getMemorySetting--) | Récupère l'option d'utilisation de la mémoire pour ces cellules. |
| [getMergedAreas()](#getMergedAreas--) | Obtient toutes les cellules fusionnées. |
| [getMergedCells()](#getMergedCells--) | Obtient la collection des cellules fusionnées. |
| [getMinColumn()](#getMinColumn--) | Indice de colonne minimum de ces cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée). |
| [getMinDataColumn()](#getMinDataColumn--) | Indice de colonne minimum de la cellule qui contient des données. |
| [getMinDataRow()](#getMinDataRow--) | Indice de ligne minimum de la cellule qui contient des données. |
| [getMinRow()](#getMinRow--) | Indice de ligne minimum de la cellule qui contient des données ou un style. |
| [getMultiThreadReading()](#getMultiThreadReading--) | Obtient si le modèle de données des cellules doit prendre en charge la lecture Multi-Thread. |
| [getOdsCellFields()](#getOdsCellFields--) | Obtient la liste des champs de ods. |
| [getPreserveString()](#getPreserveString--) | Obtient une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées sous forme de chaînes. |
| [getRanges()](#getRanges--) | Obtient la collection d'objets [Range](../../com.aspose.cells/range) créés à l'exécution. |
| [getRowEnumerator()](#getRowEnumerator--) | Obtient l'énumérateur des lignes. |
| [getRowHeight(int row)](#getRowHeight-int-) | Obtient la hauteur d'une ligne spécifiée, en points. |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | Obtient la hauteur de la ligne. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Obtient la hauteur d'une ligne spécifiée en pixels. |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | Obtient la hauteur originale de la ligne en points si la ligne est masquée. |
| [getRows()](#getRows--) | Obtient la collection d'objets [Row](../../com.aspose.cells/row) qui représente les lignes individuelles de cette feuille de calcul. |
| [getStandardHeight()](#getStandardHeight--) | Obtient la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [getStandardHeightInch()](#getStandardHeightInch--) | Obtient la hauteur de ligne par défaut dans cette feuille de calcul, en pouces. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Obtient la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [getStandardWidth()](#getStandardWidth--) | Obtient la largeur de colonne par défaut dans la feuille de calcul, en caractères. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Obtient la largeur de colonne par défaut dans la feuille de calcul, en pouces. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Obtient la largeur de colonne par défaut dans la feuille de calcul, en pixels. |
| [getStyle()](#getStyle--) | Obtient le style par défaut de la feuille de calcul. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Obtenez la largeur dans différents types de vue. |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | Obtient la hauteur d'une ligne spécifiée. |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Regroupe les colonnes. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Regroupe les colonnes. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Regroupe les lignes. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Regroupe les lignes. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Masque une colonne. |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | Masque plusieurs colonnes. |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | Réduit les lignes/colonnes groupées. |
| [hideRow(int row)](#hideRow-int-) | Masque une ligne. |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | Masque plusieurs lignes. |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | Importe un tableau de double dans une feuille de calcul. |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | Importe un tableau à deux dimensions de double dans une feuille de calcul. |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | Importe un tableau d'entier dans une feuille de calcul. |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | Importe un tableau à deux dimensions d'entier dans une feuille de calcul. |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | Importe un tableau de chaînes dans une feuille de calcul. |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | Importe un tableau à deux dimensions de chaînes dans une feuille de calcul. |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | Importe une ArrayList de données dans une feuille de calcul. |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | Importe un fichier CSV dans les cellules. |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | Importe un fichier CSV dans les cellules. |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | Importe un fichier CSV dans les cellules. |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | Importe un fichier CSV dans les cellules. |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | Importe des objets personnalisés. |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | Importe des objets personnalisés. |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | Importe des données d'un tableau de données personnalisé. |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | Importe un tableau de formules dans une feuille de calcul. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | Importe un tableau de données dans une feuille de calcul. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | Importe un tableau de données dans une feuille de calcul. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | Importe des données d'un objet ResultSet dans la feuille de calcul. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | Importe des données d'un objet ResultSet dans la feuille de calcul. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | Importe des données d'un objet ResultSet dans la feuille de calcul. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | Importe des données d'un objet ResultSet dans la feuille de calcul. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | Importe des données d'un objet ResultSet dans la feuille de calcul. |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | Importe des données d'un objet ResultSet dans la feuille de calcul. |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | Importe des données d'un objet ResultSet dans la feuille de calcul. |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | Importe des données d'un objet ResultSet dans la feuille de calcul. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | Importe un tableau à deux dimensions de données dans une feuille de calcul. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | Importe un tableau à deux dimensions de données dans une feuille de calcul. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | Importe un tableau à deux dimensions de données dans une feuille de calcul. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | Importe un tableau à deux dimensions de données dans une feuille de calcul. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Insère une nouvelle colonne dans la feuille de calcul. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Insère une nouvelle colonne dans la feuille de calcul. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Insère plusieurs colonnes dans la feuille de calcul. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Insère plusieurs colonnes dans la feuille de calcul. |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | Insère plusieurs colonnes dans la feuille de calcul. |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | Insérer la plage découpée. |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [insertRow(int rowIndex)](#insertRow-int-) | Insère une nouvelle ligne dans la feuille de calcul. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Insère plusieurs lignes dans la feuille de calcul. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Insère plusieurs lignes dans la feuille de calcul. |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | Insère plusieurs lignes dans la feuille de calcul. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Vérifie si la colonne donnée est vide (ne contient aucune donnée). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Vérifie si une colonne à l'index donné est masquée. |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | Indique que la hauteur de la ligne et la hauteur de police par défaut correspondent |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | Indique si la ligne est masquée par défaut. |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | Vérifie si la plage peut être supprimée. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Vérifie si une ligne à l'index donné est masquée. |
| [iterator()](#iterator--) | Obtient l'énumérateur des cellules. |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | Lien vers une carte XML. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | Déplace la plage. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | Supprime les lignes en double dans la feuille. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Supprime les valeurs en double dans la plage. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | Supprime les données en double de la plage. |
| [removeFormulas()](#removeFormulas--) | Supprime toutes les formules et les remplace par la valeur de la formule. |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | Récupère les paramètres de sous‑total de la plage. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Définit la largeur de la colonne spécifiée en mode normal. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Définit la largeur de la colonne en pouces en mode normal. |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | Définit la largeur de la colonne en pixels en mode normal. |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | Indique que la hauteur de la ligne et la hauteur de police par défaut correspondent |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | Indique si la ligne est masquée par défaut. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Définit l'option d'utilisation de la mémoire pour ces cellules. |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | Définit si le modèle de données des cellules doit prendre en charge la lecture multithread. |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | Définit une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées en tant que chaînes. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Définit la hauteur de la ligne spécifiée. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Définit la hauteur de la ligne en unités de pouces. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Définit la hauteur de la ligne en unités de pixels. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Définit la hauteur de ligne par défaut dans cette feuille de calcul, en unités de points. |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | Définit la hauteur de ligne par défaut dans cette feuille de calcul, en unités de pouces. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Définit la hauteur de ligne par défaut dans cette feuille de calcul, en unités de pixels. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Définit la largeur de colonne par défaut dans la feuille de calcul, en unités de caractères. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Définit la largeur de colonne par défaut dans la feuille de calcul, en unités de pouces. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Définit la largeur de colonne par défaut dans la feuille de calcul, en unités de pixels. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Définit le style par défaut de la feuille de calcul. |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | Définit la largeur de la colonne dans différentes vues. |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | Développe les lignes/colonnes groupées. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | Crée des sous‑totaux pour la plage. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | Crée des sous‑totaux pour la plage. |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | Divise le contenu de la colonne spécifiée en plusieurs colonnes.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Annule la fusion d’une plage spécifiée de cellules fusionnées. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Dégroupe les colonnes. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Dégroupe les lignes. |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | Dégroupe les lignes. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Affiche une colonne |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | Affiche plusieurs colonnes. |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | Affiche une ligne. |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | Affiche les lignes cachées. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


Ajoute une référence d'objet de plage aux cellules

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | L’objet de plage sera contenu dans les cellules |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


Applique des formats à une colonne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | L'index de colonne. |
| style | [Style](../../com.aspose.cells/style) | L'objet de style qui sera appliqué. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Drapeaux qui indiquent les propriétés de formatage appliquées. |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


Applique des formats à une ligne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| style | [Style](../../com.aspose.cells/style) | L'objet de style qui sera appliqué. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Drapeaux qui indiquent les propriétés de formatage appliquées. |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applique des formats à une feuille de calcul entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'objet de style qui sera appliqué. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Drapeaux qui indiquent les propriétés de formatage appliquées. |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


Obtient l'élément [Cell](../../com.aspose.cells/cell) ou null à l'indice de ligne et de colonne de cellule spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne |
| colonne | int | Indice de colonne |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


Obtient l'élément [Column](../../com.aspose.cells/column) ou null à l'indice de colonne spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | L'index de colonne. |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


Obtient l'élément [Row](../../com.aspose.cells/row) ou null à l'indice de ligne de cellule spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Efface toutes les données de la feuille de calcul.

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


Efface le contenu d'une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Plage à effacer. |

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

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


Efface le formatage d'une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Plage à effacer. |

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

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


Efface toutes les plages fusionnées.

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


Efface le contenu et le formatage d'une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Plage à effacer. |

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

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


Convertit toutes les données de type chaîne de la feuille de calcul en valeur numérique si possible.

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Copie les données et les formats d'une colonne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L’objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | int | Indice de colonne source. |
| destinationColumnIndex | int | Indice de colonne de destination. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Copie les données et les formats de colonnes entières.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L’objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | int | Indice de colonne source. |
| destinationColumnIndex | int | Indice de colonne de destination. |
| columnNumber | int | Le numéro de colonne copié. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


Copie les données et les formats d'une colonne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L’objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | int | Indice de colonne source. |
| destinationColumnIndex | int | Indice de colonne de destination. |
| columnNumber | int | Le numéro de colonne copié. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | les options de collage. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


Copie les données et les formats de toutes les colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L’objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | int | Indice de colonne source. |
| sourceTotalColumns | int | Le nombre de colonnes source. |
| destinationColumnIndex | int | Indice de colonne de destination. |
| destinationTotalColumns | int | Le nombre de colonnes de destination. |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Copie les données et les formats d'une ligne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L’objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | int | Indice de ligne source. |
| destinationRowIndex | int | Indice de ligne de destination. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Copie les données et les formats de certaines lignes entières.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L’objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | int | Indice de ligne source. |
| destinationRowIndex | int | Indice de ligne de destination. |
| rowNumber | int | Le numéro de ligne copié. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


Copie les données et les formats de certaines lignes entières.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | L’objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | int | Indice de ligne source. |
| destinationRowIndex | int | Indice de ligne de destination. |
| rowNumber | int | Le numéro de ligne copié. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Les options de copie. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


Copie les données et les formats de certaines lignes entières.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | L’objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | int | Indice de ligne source. |
| destinationRowIndex | int | Indice de ligne de destination. |
| rowNumber | int | Le numéro de ligne copié. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Les options de copie. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | les options de collage. |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


Crée un objet [Range](../../com.aspose.cells/range) à partir de lignes de cellules ou de colonnes de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Indice de première ligne ou indice de première colonne, basé sur zéro. |
| number | int | Nombre total de lignes ou de colonnes, basé sur un. |
| isVertical | boolean | Vrai - Plage créée à partir des colonnes de cellules. Faux - Plage créée à partir des lignes de cellules. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Crée un objet [Range](../../com.aspose.cells/range) à partir d'une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Première ligne de cette plage |
| firstColumn | int | Première colonne de cette plage |
| totalRows | int | Nombre de lignes |
| totalColumns | int | Nombre de colonnes |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


Crée un objet [Range](../../com.aspose.cells/range) à partir d'une adresse de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| adresse | java.lang.String | L'adresse de la plage. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


Crée un objet [Range](../../com.aspose.cells/range) à partir d'une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| upperLeftCell | java.lang.String | Nom de la cellule en haut à gauche. |
| lowerRightCell | java.lang.String | Nom de la cellule en bas à droite. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Supprime toutes les colonnes vides qui ne contiennent aucune donnée.

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


Supprime toutes les colonnes vides qui ne contiennent aucune donnée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Les options de suppression de la plage. |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Supprime toutes les lignes vides qui ne contiennent aucune donnée ou aucun autre objet.

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


Supprime toutes les lignes vides qui ne contiennent aucune donnée ou certains objets spéciaux tels que les commentaires visibles, les tableaux croisés dynamiques.

**Remarks**

Pour les lignes vides qui seront supprimées, il ne suffit pas que [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) soit vrai, il faut également qu'aucun commentaire visible ne soit défini pour aucune cellule de ces lignes, et qu'aucun tableau croisé dynamique dont la plage intersecte celles‑ci ne soit présent.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Les options de suppression de la plage. |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Supprime une colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de la colonne à supprimer. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Supprime une colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de la colonne à supprimer. |
| updateReference | boolean | Indique si les références doivent être mises à jour dans les autres feuilles de calcul. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Supprime plusieurs colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de la première colonne à supprimer. |
| totalColumns | int | Nombre de colonnes à supprimer. |
| updateReference | boolean | Indique si les références doivent être mises à jour dans les autres feuilles de calcul. |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


Supprime plusieurs colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de la première colonne à supprimer. |
| totalColumns | int | Nombre de colonnes à supprimer. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Options pour l'opération de suppression |

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
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Option de déplacement des cellules. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Supprime une ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de la ligne à supprimer. |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


Supprime une ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de la ligne à supprimer. |
| updateReference | boolean | Indique si les références doivent être mises à jour dans les autres feuilles de calcul. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Supprime plusieurs lignes.

**Remarks**

Si la plage supprimée contient la partie supérieure (pas la totalité) du tableau (ListObject), la plage ne peut pas être supprimée et aucune action ne sera effectuée. Cela fonctionne de la même manière avec MS Excel.

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
| rowIndex | int | Indice de la première ligne à supprimer. |
| totalRows | int | Nombre de lignes à supprimer. |
| updateReference | boolean | Indique si les références doivent être mises à jour dans les autres feuilles de calcul. |

**Returns:**
boolean -
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


Supprime plusieurs lignes dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de la première ligne à supprimer. |
| totalRows | int | Nombre de lignes à supprimer. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Options pour l'opération de suppression |

**Returns:**
boolean -
### dispose() {#dispose--}
```
public void dispose()
```


Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées.

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


Obtient la dernière cellule de cette colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


Obtient la dernière cellule avec l'index de colonne maximal dans cette plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| endRow | int | Indice de ligne de fin. |
| startColumn | int | Indice de colonne de départ. |
| endColumn | int | Indice de colonne de fin. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


Obtient la dernière cellule de cette ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de ligne. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


Obtient la dernière cellule avec l'index de ligne maximal dans cette plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| endRow | int | Indice de ligne de fin. |
| startColumn | int | Indice de colonne de départ. |
| endColumn | int | Indice de colonne de fin. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
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


Exporte les données de la collection [Cells](../../com.aspose.cells/cells) vers un objet tableau à deux dimensions.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Numéro de ligne de la première cellule à exporter. |
| firstColumn | int | Numéro de colonne de la première cellule à exporter |
| totalRows | int | Nombre de lignes à exporter |
| totalColumns | int | Nombre de colonnes à exporter |

**Returns:**
java.lang.Object[][] - Objet tableau de valeurs de cellules exportées.
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exporte le type de valeur des cellules de la collection [Cells](../../com.aspose.cells/cells) vers un objet tableau à deux dimensions.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Numéro de ligne de la première cellule à exporter. |
| firstColumn | int | Numéro de colonne de la première cellule à exporter |
| totalRows | int | Nombre de lignes à exporter. |
| totalColumns | int | Nombre de colonnes à exporter. |

**Returns:**
int[][] - [CellValueType](../../com.aspose.cells/cellvaluetype). Tableau exporté représentant les types de valeurs de cellules.
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


Trouve la cellule contenant l'objet d'entrée.

**Remarks**

Renvoie null (Nothing) si aucune cellule n’est trouvée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| quoi | java.lang.Object | L’objet à rechercher. Le type doit être int, double, DateTime, string, bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Cellule précédente contenant le même objet. Ce paramètre peut être défini sur null si la recherche commence depuis le début. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


Trouve la cellule contenant l'objet d'entrée.

**Remarks**

Renvoie null (Nothing) si aucune cellule n’est trouvée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| quoi | java.lang.Object | L’objet à rechercher. Le type doit être int, double, DateTime, string, bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Cellule précédente contenant le même objet. Ce paramètre peut être défini sur null si la recherche commence depuis le début. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Options de recherche |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


Obtient l'élément [Cell](../../com.aspose.cells/cell) aux index de ligne et de colonne de cellule spécifiés.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| colonne | int | Indice de colonne. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


Obtient l'élément [Cell](../../com.aspose.cells/cell) au nom de cellule spécifié.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de la cellule, incluant sa lettre de colonne et son numéro de ligne, par exemple A5. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


Obtient le style d'affichage de la cellule donnée.

**Remarks**

Identique à [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), et de même en utilisant [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) pour [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | indice de ligne de la cellule donnée |
| colonne | int | colonne de la cellule donnée |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


Obtient le style d'affichage de la cellule donnée.

**Remarks**

Si la cellule est également affectée par d’autres paramètres tels que le formatage conditionnel, les objets de liste, etc., le style d’affichage peut être différent de celui de [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-). Et comme ces paramètres peuvent également être appliqués à des cellules vides (inexistantes), l’utilisation de cette méthode permet d’éviter l’instanciation de ces cellules vides, ce qui améliore les performances par rapport à l’obtention de l’instance Cell via Cells puis à l’appel de [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | indice de ligne de la cellule donnée |
| colonne | int | colonne de la cellule donnée |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Indique quelles bordures doivent être vérifiées et ajustées en fonction des bordures des cellules adjacentes. Veuillez consulter la description du même paramètre de [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


Obtenez le style de la cellule donnée.

**Remarks**

Le style renvoyé est uniquement celui défini pour la cellule ou hérité de la ligne/colonne de la cellule, il n’inclut pas les propriétés appliquées par d’autres paramètres tels que les formats conditionnels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | indice de ligne |
| colonne | int | colonne |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


Récupère toutes les cellules qui contiennent une image intégrée.

**Remarks**

S’il n’y a aucune image définie comme "Place in Cell" dans cette feuille de calcul, null sera renvoyé.

**Returns:**
java.util.Iterator - Énumérateur pour parcourir tous les objets Cell contenant une image intégrée
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnOriginalWidthPoint(int column) {#getColumnOriginalWidthPoint-int-}
```
public double getColumnOriginalWidthPoint(int column)
```


Récupère la hauteur d'origine de la colonne en points si la colonne est masquée

**Remarks**

NOTE : Cette méthode est désormais obsolète. Veuillez plutôt utiliser la méthode Cells.GetColumnWidth(int ,bool , CellsUnitType ). Cette méthode sera supprimée 12 mois après avril 2024. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | L'index de ligne. |

**Returns:**
double - Largeur de la colonne en vue normale.
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Récupère la largeur (en nombre de caractères) de la colonne spécifiée en vue normale

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne |

**Returns:**
double - Largeur de la colonne. Dans une feuille de calcul, la largeur de colonne est mesurée en nombre de caractères correspondant à la largeur maximale d’un chiffre des nombres 0~9 telle qu’elle apparaît dans la police du style normal.
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


Récupère la largeur de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | L'index de colonne. |
| isOriginal | boolean | Indique s’il faut obtenir la largeur originale. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). |

**Returns:**
double -
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Récupère la largeur de la colonne spécifiée en vue normale, en pouces.

**Remarks**

NOTE : Cette méthode est désormais obsolète. Veuillez plutôt utiliser la méthode Cells.GetColumnWidth(int ,bool , CellsUnitType ). Cette méthode sera supprimée 12 mois après avril 2024. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne |

**Returns:**
double - Largeur de la colonne en vue normale.
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Récupère la largeur de la colonne spécifiée en vue normale, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne |

**Returns:**
int - Largeur de la colonne en vue normale.
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


Récupère la largeur de la colonne spécifiée en vue normale, en pixels.

**Remarks**

NOTE : Cette méthode est désormais obsolète. Veuillez plutôt utiliser la méthode Cells.GetColumnWidth(int ,bool , CellsUnitType ). Cette méthode sera supprimée 12 mois après avril 2024. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne |
| original | boolean | Indique s’il faut renvoyer la largeur originale même lorsque la colonne est masquée |

**Returns:**
int - Largeur de la colonne en vue normale.
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


Récupère la collection d'objets [Column](../../com.aspose.cells/column) qui représente les colonnes individuelles dans cette feuille de calcul.

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Récupère le nombre total d'objets Cell instanciés.

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


Récupère le nombre total d'objets Cell instanciés.

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


Obtenez toutes les cellules qui font référence à la cellule spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indique s’il faut vérifier les autres feuilles de calcul |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
com.aspose.cells.Cell[] -
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


Récupère toutes les cellules dont le résultat calculé dépend de la cellule spécifique.

**Remarks**

Pour utiliser cette méthode, assurez‑vous que le classeur a bien la valeur true pour [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) et qu’il a été entièrement calculé avec ce paramètre. S’il n’existe aucune référence de formule à cette cellule, null sera renvoyé. Pour plus de détails et un exemple, veuillez consulter [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne de la cellule spécifique |
| colonne | int | Indice de colonne de la cellule spécifique. |
| recursive | boolean | Indique si elle renvoie les dépendants qui ne font pas référence directement à la cellule spécifique mais font référence à d'autres feuilles de cette cellule. |

**Returns:**
java.util.Iterator - Énumérateur pour parcourir tous les dépendants (objets Cell).
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Récupère la première cellule de cette feuille de calcul.

**Remarks**

Renvoie null s'il n'y a aucune donnée dans la feuille de calcul.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


Récupère l'index de la première ligne de la cellule qui contient des données dans la colonne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |

**Returns:**
int - indice de la première ligne.
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


Récupère le niveau de contour (à partir de zéro) de la colonne.

**Remarks**

Si la colonne n'est pas groupée, renvoie zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | L'index de colonne |

**Returns:**
int - Le niveau de contour de la colonne
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


Récupère le niveau de contour (à partir de zéro) de la ligne.

**Remarks**

Si la ligne n'est pas groupée, renvoie zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | L'index de ligne. |

**Returns:**
int - Le niveau de contour (basé sur zéro) de la ligne.
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Récupère la dernière cellule de cette feuille de calcul.

**Remarks**

Renvoie null s'il n'y a aucune donnée dans la feuille de calcul.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


Récupère l'index de la dernière ligne de la cellule qui contient des données dans la colonne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |

**Returns:**
int - indice de la dernière ligne.
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Indice maximal de colonne des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée).

**Remarks**

Renvoie -1 s'il n'y a aucune cellule instanciée.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Indice maximal de colonne de la cellule qui contient des données.

**Remarks**

\-1 sera renvoyé s'il n'existe aucune cellule contenant des données. Cette propriété doit itérer et vérifier toutes les cellules d'une feuille de calcul dynamiquement, ce qui consomme du temps et ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Indice maximal de ligne de la cellule qui contient des données.

**Remarks**

Renvoie -1 s'il n'existe aucune cellule contenant des données. Cette propriété doit itérer et vérifier les cellules et les lignes dynamiquement, ce qui consomme du temps et ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


Récupère la plage maximale qui inclut les données, les cellules fusionnées et les formes.

**Remarks**

Renvoie null si la feuille de calcul est vide depuis Aspose.Cells 21.5.2.

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


Récupère le niveau de contour maximal des colonnes groupées (à partir de zéro).

**Returns:**
int - Le niveau de contour maximal des colonnes groupées (basé sur zéro)
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


Récupère le niveau de contour maximal des lignes groupées (à partir de zéro).

**Returns:**
int - Le niveau de contour maximal des lignes groupées (basé sur zéro)
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Indice maximal de ligne de la cellule qui contient des données ou un style.

**Remarks**

Renvoie -1 s'il n'existe aucune cellule contenant des données ou un style dans la feuille de calcul. Cette propriété doit itérer et vérifier les cellules et les lignes dynamiquement, ce qui consomme du temps et ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Récupère l'option d'utilisation de la mémoire pour ces cellules.

Voir [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Limites notables et opérations recommandées pour certains modes :

| Mode | Remarques | Pris en charge |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Lorsque ce mode est utilisé pour une feuille de calcul dans un classeur, [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) doit être appelé à la fin du travail pour libérer toutes les ressources telles que les fichiers temporaires. |
 
L'accès aléatoire aux cellules entraîne de mauvaises performances car les données doivent être lues/mises à jour de manière aléatoire et répétée (le pointeur dans le fichier sera donc modifié en conséquence et des opérations d'E/S seront requises de façon répétée). Si possible, veuillez toujours accéder aux données de manière séquentielle (ligne par ligne).
 
Lorsque les données d'une ligne/cellule sont modifiées, les données des autres cellules/lignes peuvent également être affectées (par exemple, les données sont déplacées/shiftées vers d'autres emplacements pour allouer suffisamment d'espace aux données modifiées). Ainsi, chaque modification de chaque donnée nécessite la synchronisation des autres objets existants (tels que les objets Row ou Cell). Donc, pour obtenir de meilleures performances, veuillez ne pas maintenir plusieurs Rows/Cells en même temps. Les traiter un par un réduira la synchronisation des données, ce qui améliorera légèrement les performances. | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


Obtient toutes les cellules fusionnées.

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Obtient la collection des cellules fusionnées.

**Remarks**

NOTE : Cette méthode est désormais obsolète. Veuillez plutôt utiliser la méthode Cells.GetMergedAreas(). Cette méthode sera supprimée 12 mois plus tard, depuis novembre 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Indice de colonne minimum de ces cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée).

**Remarks**

Cette propriété doit itérer et vérifier les cellules et les lignes de manière dynamique, il s'agit donc d'un processus gourmand en temps et elle ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Indice de colonne minimum de la cellule qui contient des données.

**Remarks**

\-1 sera renvoyé s'il n'existe aucune cellule contenant des données. Cette propriété doit itérer et vérifier toutes les cellules d'une feuille de calcul dynamiquement, ce qui consomme du temps et ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Indice de ligne minimum de la cellule qui contient des données.

**Remarks**

Renvoie -1 s'il n'existe aucune cellule contenant des données. Cette propriété doit itérer et vérifier les cellules et les lignes dynamiquement, ce qui consomme du temps et ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Indice de ligne minimum de la cellule qui contient des données ou un style.

**Remarks**

Cette propriété doit itérer et vérifier les cellules et les lignes de manière dynamique, il s'agit donc d'un processus gourmand en temps et elle ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


Obtient si le modèle de données des cellules doit prendre en charge la lecture multi‑thread. La valeur par défaut de cette propriété est false.

**Remarks**

S'il y a plusieurs threads qui lisent les objets Row/Cell dans cette collection simultanément, cette propriété doit être définie sur true, sinon des résultats inattendus peuvent être produits. Prendre en charge la lecture Multi‑Thread peut dégrader les performances d'accès aux objets Row/Cell de cette collection. Veuillez noter que certaines fonctionnalités ne peuvent pas prendre en charge la lecture Multi‑Thread, comme le formatage des valeurs (par [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), etc.). Ainsi, même si cette propriété est définie sur true, ces API peuvent encore donner des résultats inattendus lors de la lecture Multi‑Thread.

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


Obtient la liste des champs de ods.

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


Obtient une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées sous forme de chaînes. La valeur par défaut est false.

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


Obtient la collection d'objets [Range](../../com.aspose.cells/range) créés à l'exécution.

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Obtient l'énumérateur des lignes.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode RowCollection.GetEnumerator(). Cette méthode sera supprimée 12 mois après mai 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.util.Iterator - L'énumérateur de lignes.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Obtient la hauteur d'une ligne spécifiée, en points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne |

**Returns:**
double - Hauteur de la ligne
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


Obtient la hauteur de la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| isOriginal | boolean | Indique si la hauteur originale de la ligne est renvoyée ou 0 pour une ligne masquée. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). Type d'unité de la valeur de hauteur renvoyée |

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
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


Obtient la hauteur originale de la ligne en points si la ligne est masquée.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Cells.GetRowHeight(int,bool,CellsUnitType). Cette méthode sera supprimée 12 mois après avril 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |

**Returns:**
double -
### getRows() {#getRows--}
```
public RowCollection getRows()
```


Obtient la collection d'objets [Row](../../com.aspose.cells/row) qui représente les lignes individuelles de cette feuille de calcul.

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Obtient la hauteur de ligne par défaut dans cette feuille de calcul, en points.

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


Obtient la hauteur de ligne par défaut dans cette feuille de calcul, en pouces.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Obtient la hauteur de ligne par défaut dans cette feuille de calcul, en pixels.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Obtient la largeur de colonne par défaut dans la feuille de calcul, en caractères.

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
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtient le style par défaut de la feuille de calcul.

**Returns:**
[Style](../../com.aspose.cells/style)
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
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


Obtient la hauteur d'une ligne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |

**Returns:**
double - Hauteur de la ligne.
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


Obtient la hauteur d'une ligne spécifiée en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne |

**Returns:**
double - Hauteur de la ligne
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

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Regroupe les lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de ligne à regrouper. |
| lastIndex | int | Le dernier indice de ligne à regrouper. |
| isHidden | boolean | Spécifie si les lignes regroupées sont masquées. |

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

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


Masque plusieurs colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| totalColumns | int | Numéro de colonne. |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


Réduit les lignes/colonnes groupées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isVertical | boolean | True, réduire les lignes regroupées. |
| index | int | L'index de ligne/colonne |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Masque une ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


Masque plusieurs lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| totalRows | int | Le numéro de ligne. |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


Importe un tableau de double dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| doubleArray | double[] | Tableau double. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| isVertical | boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


Importe un tableau à deux dimensions de double dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| doubleArray | double[][] | Tableau double à deux dimensions. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


Importe un tableau d'entier dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| intArray | int[] | Tableau d'entiers. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| isVertical | boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


Importe un tableau à deux dimensions d'entier dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| intArray | int[][] | Tableau d'entiers à deux dimensions. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importe un tableau de chaînes dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringArray | java.lang.String[] | Tableau de chaînes. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| isVertical | boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


Importe un tableau à deux dimensions de chaînes dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringArray | java.lang.String[][] | Tableau de chaînes à deux dimensions. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


Importe une ArrayList de données dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arrayList | java.util.ArrayList | Données arraylist. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| isVertical | boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importe un fichier CSV dans les cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux du fichier CSV. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Les options de chargement pour la lecture du fichier texte |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importe un fichier CSV dans les cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux du fichier CSV. |
| splitter | java.lang.String | Le séparateur |
| convertNumericData | boolean | Indique si la chaîne dans le fichier texte est convertie en données numériques. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


Importe un fichier CSV dans les cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier CSV. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Les options de chargement pour la lecture du fichier texte |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Importe un fichier CSV dans les cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier CSV. |
| splitter | java.lang.String | Le séparateur |
| convertNumericData | boolean | Indique si la chaîne dans le fichier texte est convertie en données numériques. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


Importe des objets personnalisés.

**Remarks**

Les objets personnalisés doivent être du même type.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| liste | java.util.Collection | L'objet personnalisé |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Les options d'importation. |

**Returns:**
int - Nombre total de lignes importées.
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


Importe des objets personnalisés.

**Remarks**

Les objets personnalisés doivent être du même type.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| liste | java.util.Collection | L'objet personnalisé |
| propertyNames | java.lang.String[] | Les noms de propriétés. Si c'est nul, nous importerons toutes les propriétés de l'objet. |
| isPropertyNameShown | boolean | Indique si le nom de la propriété sera importé dans la première ligne. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| rowNumber | int | Nombre de lignes à importer. |
| insertRows | boolean | Indique si des lignes supplémentaires sont ajoutées pour adapter les données. |
| dateFormatString | java.lang.String | Chaîne de format de date pour les cellules. |
| convertStringToNumber | boolean | Indique si cette méthode tentera de convertir la chaîne en nombre. |

**Returns:**
int - Nombre total de lignes importées.
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


Importe des données d'un tableau de données personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | Le tableau de données personnalisé. |
| firstRow | int | Indice de la première ligne. |
| firstColumn | int | Indice de la première colonne. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Les options d'importation |

**Returns:**
int -
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Importe un tableau de formules dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringArray | java.lang.String[] | Tableau de formules. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| isVertical | boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


Importe un tableau de données dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[] | Tableau de données. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| isVertical | boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


Importe un tableau de données dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[] | Tableau de données. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| isVertical | boolean | Spécifie d'importer les données verticalement ou horizontalement. |
| ignorer | int | Nombre de lignes ou de colonnes ignorées. |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


Importe des données d'un objet ResultSet dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'objet ResultSet à partir duquel importer. |
| rowIndex | int | indice de ligne de départ dans la feuille de calcul. |
| columnIndex | int | indice de colonne de départ dans la feuille de calcul. |
| isFieldNameShown | boolean | Indique si le nom de champ du resultset sera importé dans la première ligne. |

**Returns:**
int - nombre de lignes réellement importées.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importe des données d'un objet ResultSet dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'objet ResultSet à partir duquel importer. |
| rowIndex | int | indice de ligne de départ dans la feuille de calcul. |
| columnIndex | int | indice de colonne de départ dans la feuille de calcul. |
| isFieldNameShown | boolean | Indique si le nom de champ du resultset sera importé dans la première ligne. |
| customDateFormatString | java.lang.String | Chaîne de format de date pour les cellules contenant une valeur de date. |
| convertStringToNumber | boolean | Indique si cette méthode tentera de convertir la chaîne en nombre. |

**Returns:**
int - nombre de lignes réellement importées.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


Importe des données d'un objet ResultSet dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'objet ResultSet à partir duquel importer. |
| rowIndex | int | indice de ligne de départ dans la feuille de calcul. |
| columnIndex | int | indice de colonne de départ dans la feuille de calcul. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Les options d'importation |

**Returns:**
int - nombre de lignes réellement importées.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importe des données d'un objet ResultSet dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'objet ResultSet à partir duquel importer. |
| rowIndex | int | indice de ligne de départ dans la feuille de calcul. |
| columnIndex | int | indice de colonne de départ dans la feuille de calcul. |
| rowNum | int | nombre de lignes à importer. -1 pour importer tous les enregistrements du resultset donné. |
| columnNum | int | nombre de colonnes à importer. -1 pour importer toutes les colonnes du resultset donné. |
| isFieldNameShown | boolean | Indique si le nom de champ du resultset sera importé dans la première ligne. |

**Returns:**
int - nombre de lignes réellement importées.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Importe des données d'un objet ResultSet dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'objet ResultSet à partir duquel importer. |
| rowIndex | int | indice de ligne de départ dans la feuille de calcul. |
| columnIndex | int | indice de colonne de départ dans la feuille de calcul. |
| rowNum | int | nombre de lignes à importer. -1 pour importer tous les enregistrements du resultset donné. |
| columnNum | int | nombre de colonnes à importer. -1 pour importer toutes les colonnes du resultset donné. |
| isFieldNameShown | boolean | Indique si le nom de champ du resultset sera importé dans la première ligne. |
| customDateFormatString | java.lang.String | Chaîne de format de date pour les cellules contenant une valeur de date. |
| convertStringToNumber | boolean | Indique si cette méthode tentera de convertir la chaîne en nombre. |

**Returns:**
int - nombre de lignes réellement importées.
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


Importe des données d'un objet ResultSet dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'objet ResultSet à partir duquel importer. |
| startCell | java.lang.String | nom de la cellule de départ pour insérer le resultset, par exemple "A1". |
| isFieldNameShown | boolean | Indique si le nom de champ du resultset sera importé dans la première ligne. |

**Returns:**
int - nombre de lignes réellement importées.
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


Importe des données d'un objet ResultSet dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'objet ResultSet à partir duquel importer. |
| startCell | java.lang.String | nom de la cellule de départ pour insérer le resultset, par exemple "A1". |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | Les options d'importation |

**Returns:**
int - nombre de lignes réellement importées.
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


Importe des données d'un objet ResultSet dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | l'objet ResultSet à partir duquel importer. |
| startCell | java.lang.String | nom de la cellule de départ pour insérer le resultset, par exemple "A1". |
| rowNum | int | nombre de lignes à importer. -1 pour importer tous les enregistrements du resultset donné. |
| columnNum | int | nombre de colonnes à importer. -1 pour importer toutes les colonnes du resultset donné. |
| isFieldNameShown | boolean | Indique si le nom de champ du resultset sera importé dans la première ligne. |

**Returns:**
int - nombre de lignes réellement importées.
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


Importe un tableau à deux dimensions de données dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Tableau de données à deux dimensions. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importe un tableau à deux dimensions de données dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Tableau de données à deux dimensions. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| convertStringToNumber | boolean | Indique si cette méthode tentera de convertir la chaîne en nombre. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Importe un tableau à deux dimensions de données dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Tableau de données à deux dimensions. |
| styles | java.lang.Object[][] | Style de données à deux dimensions. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| convertStringToNumber | boolean | Indique si cette méthode tentera de convertir la chaîne en nombre. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


Importe un tableau à deux dimensions de données dans une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| objArray | java.lang.Object[][] | Tableau de données à deux dimensions. |
| styles | java.lang.Object[][] | Style de données à deux dimensions. |
| firstRow | int | Le numéro de ligne de la première cellule à importer. |
| firstColumn | int | Le numéro de colonne de la première cellule à importer. |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Options pour convertir les valeurs de chaîne |

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

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


Insère plusieurs colonnes dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |
| totalColumns | int | Le nombre de colonnes. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Les options pour l'opération d'insertion. |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


Insérer la plage découpée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | La plage découpée. |
| ligne | int | La ligne. |
| colonne | int | La colonne. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Indique comment déplacer d'autres objets de la plage cible lors de l'insertion de la plage découpée. |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


Insère une plage de cellules et décale les cellules selon l'option de décalage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Déplacer la zone. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Option de déplacement des cellules. |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


Insère une plage de cellules et décale les cellules selon l'option de décalage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Déplacer la zone. |
| shiftNumber | int | Nombre de lignes ou de colonnes à insérer. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Option de déplacement des cellules. |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Insère une plage de cellules et décale les cellules selon l'option de décalage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Déplacer la zone. |
| shiftNumber | int | Nombre de lignes ou de colonnes à insérer. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Option de déplacement des cellules. |
| updateReference | boolean | Indique si les références doivent être mises à jour dans les autres feuilles de calcul. |

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

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


Insère plusieurs lignes dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de ligne. |
| totalRows | int | Nombre de lignes à insérer. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Options pour l'opération d'insertion. |

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
### isDefaultColumnHidden() {#isDefaultColumnHidden--}
```
public boolean isDefaultColumnHidden()
```




**Returns:**
boolean
### isDefaultRowHeightMatched() {#isDefaultRowHeightMatched--}
```
public boolean isDefaultRowHeightMatched()
```


Indique que la hauteur de la ligne et la hauteur de police par défaut correspondent

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


Indique si la ligne est masquée par défaut.

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


Vérifie si la plage peut être supprimée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | L'index de ligne de départ de la plage. |
| startColumn | int | L'index de colonne de départ de la plage. |
| totalRows | int | Le nombre de lignes dans la plage. |
| totalColumns | int | Le nombre de colonnes dans la plage. |

**Returns:**
boolean -
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


Obtient l'énumérateur des cellules.

**Remarks**

Lors du parcours des éléments à l'aide de l'énumérateur retourné, la collection de cellules ne doit pas être modifiée (par exemple des opérations qui créeraient de nouvelles Cell/Row ou supprimeraient des Cell/Row existantes). Sinon, l'énumérateur pourrait ne pas être capable de parcourir correctement toutes les cellules (certains éléments pourraient être parcourus plusieurs fois ou être ignorés).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - L'énumérateur de cellules
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


Lien vers une carte XML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| mapName | java.lang.String | nom de la carte xml |
| ligne | int | ligne de la cellule de destination |
| colonne | int | colonne de la cellule de destination |
| chemin | java.lang.String | chemin de l'élément xml dans la carte xml |

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

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


Fusionne une plage de cellules spécifiée en une seule cellule.

**Remarks**

Faites référence à la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage. Si mergeConflict est vrai et que la plage fusionnée entre en conflit avec d'autres cellules fusionnées, les autres cellules fusionnées seront automatiquement supprimées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Première ligne de cette plage (index zéro) |
| firstColumn | int | Première colonne de cette plage (index zéro) |
| totalRows | int | Nombre de lignes (index à partir de 1) |
| totalColumns | int | Nombre de colonnes (base 1) |
| mergeConflict | boolean | Plages fusionnées en conflit. |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


Fusionne une plage de cellules spécifiée en une seule cellule.

**Remarks**

Faites référence à la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage. Si mergeConflict est vrai et que la plage fusionnée entre en conflit avec d'autres cellules fusionnées, les autres cellules fusionnées seront automatiquement supprimées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Première ligne de cette plage (index zéro) |
| firstColumn | int | Première colonne de cette plage (index zéro) |
| totalRows | int | Nombre de lignes (index à partir de 1) |
| totalColumns | int | Nombre de colonnes (base 1) |
| checkConflict | boolean | Indique si la vérification des cellules fusionnées intersecte d'autres cellules fusionnées |
| mergeConflict | boolean | Plages fusionnées en conflit. |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


Déplace la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | La plage qui doit être déplacée. |
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




### removeDuplicates() {#removeDuplicates--}
```
public void removeDuplicates()
```


Supprime les lignes en double dans la feuille.

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Supprime les valeurs en double dans la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ. |
| startColumn | int | La colonne de départ |
| endRow | int | L'index de la ligne de fin. |
| endColumn | int | L'index de la colonne de fin. |

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


Supprime les données en double de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ. |
| startColumn | int | La colonne de départ |
| endRow | int | L'index de la ligne de fin. |
| endColumn | int | L'index de la colonne de fin. |
| hasHeaders | boolean | Indique si la plage contient des en-têtes. |
| columnOffsets | int[] | Les décalages de colonne. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Supprime toutes les formules et les remplace par la valeur de la formule.

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


Récupère les paramètres de sous‑total de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Définit la largeur de la colonne spécifiée en mode normal.

**Remarks**

Pour les feuilles de calcul, la largeur de colonne est mesurée en nombre de caractères correspondant à la largeur maximale d'un chiffre des nombres 0~9 tels qu'ils sont rendus avec la police du style normal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| largeur | double | Largeur de la colonne en unités de caractères. La largeur de colonne doit être comprise entre 0 et 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Définit la largeur de la colonne en pouces en mode normal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| inches | double | Nombre de pouces. |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


Définit la largeur de la colonne en pixels en mode normal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| pixels | int | Nombre de pixels. |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


Indique que la hauteur de la ligne et la hauteur de police par défaut correspondent

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


Indique si la ligne est masquée par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Définit l'option d'utilisation de la mémoire pour ces cellules.

Voir [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Limites notables et opérations recommandées pour certains modes :

| Mode | Remarques | Pris en charge |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Lorsque ce mode est utilisé pour une feuille de calcul dans un classeur, [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) doit être appelé à la fin du travail pour libérer toutes les ressources telles que les fichiers temporaires. |
 
L'accès aléatoire aux cellules entraîne de mauvaises performances car les données doivent être lues/mises à jour de manière aléatoire et répétée (le pointeur dans le fichier sera donc modifié en conséquence et des opérations d'E/S seront requises de façon répétée). Si possible, veuillez toujours accéder aux données de manière séquentielle (ligne par ligne).
 
Lorsque les données d'une ligne/cellule sont modifiées, les données des autres cellules/lignes peuvent également être affectées (par exemple, les données sont déplacées/shiftées vers d'autres emplacements pour allouer suffisamment d'espace aux données modifiées). Ainsi, chaque modification de chaque donnée nécessite la synchronisation des autres objets existants (tels que les objets Row ou Cell). Donc, pour obtenir de meilleures performances, veuillez ne pas maintenir plusieurs Rows/Cells en même temps. Les traiter un par un réduira la synchronisation des données, ce qui améliorera légèrement les performances. | v25.7     |

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


Définit si le modèle de données des cellules doit prendre en charge la lecture Multi-Thread. La valeur par défaut de cette propriété est false.

**Remarks**

S'il y a plusieurs threads qui lisent les objets Row/Cell dans cette collection simultanément, cette propriété doit être définie sur true, sinon des résultats inattendus peuvent être produits. Prendre en charge la lecture Multi‑Thread peut dégrader les performances d'accès aux objets Row/Cell de cette collection. Veuillez noter que certaines fonctionnalités ne peuvent pas prendre en charge la lecture Multi‑Thread, comme le formatage des valeurs (par [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), etc.). Ainsi, même si cette propriété est définie sur true, ces API peuvent encore donner des résultats inattendus lors de la lecture Multi‑Thread.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


Définit une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées en tant que chaînes. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Définit la hauteur de la ligne spécifiée.

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

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Définit la hauteur de ligne par défaut dans cette feuille de calcul, en unités de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


Définit la hauteur de ligne par défaut dans cette feuille de calcul, en unités de pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Définit la hauteur de ligne par défaut dans cette feuille de calcul, en unités de pixels.

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

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Définit le style par défaut de la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


Définit la largeur de la colonne dans différentes vues.

**Remarks**

Si le type de vue actuel est [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW), la largeur de la colonne est identique à la largeur imprimée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | L'index de colonne. |
| pixels | int | La largeur en unité de pixels. |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


Développe les lignes/colonnes groupées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isVertical | boolean | Vrai, développe les lignes groupées. |
| index | int | L'index de ligne/colonne |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


Crée des sous‑totaux pour la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage |
| groupBy | int | Le champ à regrouper, sous forme d'offset entier basé à zéro |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). La fonction de sous-total. |
| totalList | int[] | Un tableau d'offsets de champ basés à zéro, indiquant les champs auxquels les sous-totaux sont ajoutés. |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


Crée des sous‑totaux pour la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage |
| groupBy | int | Le champ à regrouper, sous forme d'offset entier basé à zéro |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). La fonction de sous-total. |
| totalList | int[] | Un tableau d'offsets de champ basés à zéro, indiquant les champs auxquels les sous-totaux sont ajoutés. |
| replace | boolean | Indique si remplacer les sous-totaux actuels |
| pageBreaks | boolean | Indique s'il faut ajouter un saut de page entre les groupes |
| summaryBelowData | boolean | Indique s'il faut ajouter un résumé sous les données. |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


Divise le contenu de la colonne spécifiée en plusieurs colonnes..

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |
| totalRows | int | Le nombre de lignes. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Les options de division. |

**Returns:**
int - Nombre total de colonnes des valeurs divisées.
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

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


Dégroupe les lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de ligne à dégrouper. |
| lastIndex | int | Le dernier indice de ligne à dégrouper. |
| isAll | boolean | Vrai, supprime toutes les informations groupées. Sinon, supprime les informations du groupe externe. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Affiche une colonne

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| largeur | double | Largeur de colonne. |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


Affiche plusieurs colonnes.

**Remarks**

Applique la largeur de colonne uniquement aux colonnes masquées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| totalColumns | int | Numéro de colonne |
| largeur | double | Largeur de colonne. |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


Affiche une ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| hauteur | double | Hauteur de ligne. La hauteur de la ligne ne sera modifiée que lorsque la ligne est masquée et que la valeur de hauteur fournie est positive. |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


Affiche les lignes cachées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| totalRows | int | Le numéro de ligne. |
| hauteur | double | Hauteur de ligne. La hauteur de la ligne ne sera modifiée que lorsque la ligne est masquée et que la valeur de hauteur fournie est positive. |

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

