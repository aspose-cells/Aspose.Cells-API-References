---
title: "GridWorksheet"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente une seule feuille de calcul."
type: docs
url: /fr/java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class GridWorksheet extends Control
```

Encapsule l'objet qui représente une seule feuille de calcul.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | Définit la plage à laquelle l'AutoFiltre spécifié s'applique. |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | Ajouter un filtre personnalisé pour la ligne spécifiée. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Ajuste automatiquement la largeur de la colonne. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Ajuste automatiquement la largeur de la colonne. |
| [autoFitColumns()](#autoFitColumns--) |  |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Ajuste automatiquement la hauteur de la ligne. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Ajuste automatiquement la hauteur de la ligne. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Ajuste automatiquement la hauteur des lignes dans une plage rectangulaire. |
| [autoFitRows()](#autoFitRows--) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Ajuste automatiquement la hauteur des lignes dans une plage. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Calcule une formule. |
| [clearComments()](#clearComments--) | Efface tous les commentaires dans la feuille de calcul du concepteur. |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | Crée un sous-total dans la feuille. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Crée un sous-total dans la feuille. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | Définit le filtre pour la colonne. Notez que nous devons appeler AddAutoFilter avant d'appeler filterString. La chaîne de critères du filtre. Notez que nous utilisons la virgule -> \",\" comme caractère de séparation, donc la valeur de cellule que vous souhaitez filtrer ne doit pas contenir de virgule. filterString(10,\"123,456\") signifie que la colonne 10 doit contenir 123 ou 456, filterString(10,\"123\") signifie que la colonne 10 doit contenir 123. L'index de colonne est séparé par des virgules, ex. 123,456,789 ou abc |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Fige les volets à la cellule spécifiée dans la feuille de calcul. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Fige les volets à la cellule spécifiée dans la feuille de calcul. |
| [getActiveCell()](#getActiveCell--) | Obtient la cellule active dans la feuille de calcul. |
| [getBackgroundImage()](#getBackgroundImage--) | Obtient l'image d'arrière-plan de la feuille de calcul. |
| [getCells()](#getCells--) | Obtient la collection [GridCell](../../com.aspose.gridweb/gridcell). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Représente le nom de code de la feuille de calcul. |
| [getColumnCaption(int column)](#getColumnCaption-int-) | Obtient la légende de la colonne. |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | Obtient le texte de l'infobulle de l'en-tête de colonne. |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | Obtient si une colonne est en lecture seule. |
| [getComments()](#getComments--) | Obtient la collection [GridComment](../../com.aspose.gridweb/gridcomment). |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. |
| [getDisplayZeros()](#getDisplayZeros--) | Vrai si les valeurs zéro sont affichées. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Représente l'index de la première colonne visible. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Représente l'index de la première ligne visible. |
| [getFreezedPanes()](#getFreezedPanes--) | Obtient les volets figés. |
| [getGridActiveCell()](#getGridActiveCell--) | Obtient la cellule active dans la feuille de calcul. |
| [getHyperlinks()](#getHyperlinks--) | Obtient la collection [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection). |
| [getIndex()](#getIndex--) | Obtient l'index de la feuille dans la collection de feuilles de calcul. |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | Obtient si la cellule est en lecture seule. Ceci est un attribut étendu de GridWeb, il ne sera pas conservé dans le fichier Excel réel. |
| [getName()](#getName--) | Obtient le nom de la feuille de calcul. |
| [getOutlineShown()](#getOutlineShown--) | Indique si l'affichage du contour est activé. |
| [getPictures()](#getPictures--) | Obtient une collection [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--). |
| [getPivotTables()](#getPivotTables--) | Obtient les tableaux croisés dynamiques dans la feuille de calcul. |
| [getRowCaption(int row)](#getRowCaption-int-) | Obtient la légende de la ligne. |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | Obtient le texte de l'infobulle de l'en-tête de ligne. |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | Obtient si une ligne est en lecture seule. |
| [getSelected()](#getSelected--) | Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert. |
| [getShapes()](#getShapes--) | Obtient une collection [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--). |
| [getStandardHeight()](#getStandardHeight--) | Obtient la hauteur de ligne par défaut dans cette feuille, en points. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Obtient la hauteur de ligne par défaut dans cette feuille, en pixels. |
| [getTabColor()](#getTabColor--) | Représente la couleur de l'onglet de la feuille de calcul. |
| [getUniqueID()](#getUniqueID--) | Obtient l'UniqueID dans le Contrôle |
| [getValidations()](#getValidations--) | Obtient la collection des paramètres de validation des données dans la feuille de calcul. |
| [getVisible()](#getVisible--) | Indique si le nom de cette feuille est affiché dans les onglets de feuilles du contrôle. |
| [getWorkbook()](#getWorkbook--) | Obtient l'objet [GridWorkbook](../../com.aspose.gridweb/gridworkbook) de la collection de feuilles de calcul. |
| [getZoom()](#getZoom--) | Représente le facteur d'échelle en pourcentage. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Regroupe les lignes. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Obtient une valeur indiquant si les lignes de grille sont visibles. La valeur par défaut est true. |
| [isProtected()](#isProtected--) | Indique si la feuille de calcul est protégée. |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | Indique si la ligne de résumé sera positionnée sous les lignes de détail dans le plan. |
| [moveTo(int index)](#moveTo-int-) | Déplace la feuille vers un autre emplacement dans la feuille de calcul. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | Actualise les auto‑filtres pour masquer ou afficher les lignes. |
| [removeAutoFilter()](#removeAutoFilter--) | Supprime le filtre automatique de la feuille de calcul. |
| [removeSubtotal()](#removeSubtotal--) | Supprime le sous-total créé par la méthode CreateSubtotal dans la feuille. |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | Le décalage entier du champ sur lequel vous souhaitez appliquer, basé sur la première colonne de filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Définit la cellule active dans la feuille de calcul. |
| [setAllCellsEditable()](#setAllCellsEditable--) | Rend toutes les cellules modifiables. Ceci est un attribut étendu. |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Rend toutes les cellules en lecture seule. Ceci est un attribut étendu, notez que cet attribut ne peut pas être conservé dans la cellule réelle ; si vous souhaitez conserver la protection, veuillez utiliser setProtect. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Définit l'image d'arrière-plan de la feuille de calcul. |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | Définit la légende pour la colonne. Veuillez noter que c'est un attribut d'extension et qu'il ne peut pas être conservé dans le fichier Excel. |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | Définit le texte de l'infobulle de l'en-tête de colonne. |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | Définit une colonne en lecture seule afin que l'utilisateur ne puisse pas la supprimer côté client. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Vrai si les valeurs zéro sont affichées. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Rend une plage de cellules modifiable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendre toutes les cellules en lecture seule en appelant la méthode SetAllCellsReadonly. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Représente l'index de la première colonne visible. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Représente l'index de la première ligne visible. |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | Définit la cellule active dans la feuille de calcul. |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Définit une valeur indiquant si les lignes de grille sont visibles. La valeur par défaut est true. |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | Définit si la cellule est en lecture seule. Ceci est un attribut étendu de GridWeb, il ne sera pas conservé dans le fichier Excel réel. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la feuille de calcul. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Indique si l'affichage du contour est activé. |
| [setProtect()](#setProtect--) | Protège la feuille de calcul. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Rend une plage de cellules en lecture seule. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Commencez par rendre toutes les cellules modifiables en appelant la méthode SetAllCellsEditable. |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | Définit la légende pour la ligne. |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | Définit le texte de l'infobulle de l'en-tête de ligne. |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | Définit une ligne en lecture seule afin que l'utilisateur ne puisse pas la supprimer côté client. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Définit la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | Indique si la ligne de résumé sera positionnée sous les lignes de détail dans le plan. |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | Représente la couleur de l'onglet de la feuille de calcul. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indique si le nom de cette feuille est affiché dans les onglets de feuilles du contrôle. |
| [setZoom(int value)](#setZoom-int-) | Représente le facteur d'échelle en pourcentage. |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | Déverrouille les volets dans la feuille de calcul. |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | Dégroupe les lignes. |
| [unProtect()](#unProtect--) | Supprime la protection de la feuille de calcul. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


Définit la plage à laquelle l'AutoFiltre spécifié s'applique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| startColumn | int | Indice de colonne de départ. |
| endColumn | int | Index de la colonne de fin. |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


Ajouter un filtre personnalisé pour la ligne spécifiée.

**Remarks**

La chaîne de critères de filtre. Notez que nous utilisons , et ; comme caractères de séparation, donc la valeur de la cellule ne doit pas contenir ces caractères de séparation. Ci-dessous les exemples de chaînes de critères //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int |  |
| critère | java.lang.String |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Ajuste automatiquement la largeur de la colonne.

**Remarks**

AutoFitColumn est une fonction imprécise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Ajuste automatiquement la largeur de la colonne.

**Remarks**

Cette méthode ajuste automatiquement une ligne en fonction du contenu d'une plage de cellules dans la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |
| firstRow | int | Indice de la première ligne. |
| lastRow | int | Indice de la dernière ligne. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```




### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Ajuste automatiquement la hauteur de la ligne.

**Remarks**

AutoFitRow est une fonction imprécise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de ligne. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Ajuste automatiquement la hauteur de la ligne.

**Remarks**

Cette méthode ajuste automatiquement une ligne en fonction du contenu d'une plage de cellules dans la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | Indice de ligne. |
| firstColumn | int | Indice de la première colonne. |
| lastColumn | int | Dernier indice de colonne. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Ajuste automatiquement la hauteur des lignes dans une plage rectangulaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| endRow | int | Indice de ligne de fin. |
| startColumn | int | Indice de colonne de départ. |
| endColumn | int | Indice de colonne de fin. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Ajuste automatiquement toutes les lignes de cette feuille de calcul.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Ajuste automatiquement toutes les lignes de cette feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| onlyAuto | boolean | True, n'ajuste automatiquement la hauteur de la ligne que lorsque la hauteur de la ligne n'est pas personnalisée. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Ajuste automatiquement la hauteur des lignes dans une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| endRow | int | Indice de ligne de fin. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Calcule une formule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object -
### clearComments() {#clearComments--}
```
public void clearComments()
```


Efface tous les commentaires dans la feuille de calcul du concepteur.

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


Copie le contenu et les formats d'une autre feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Feuille de calcul source. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
```


Crée un sous-total dans la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnNameRowIndex | int | L'index de ligne de la ligne de nom de colonne. |
| dataRows | int | Le nombre de lignes de données. |
| groupByColumnIndex | int | L'index de colonne de la colonne à regrouper. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Le type de fonction de sous-total. |
| subtotalColumnIndexList | int[] | Les index de colonnes à sous-totaliser. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Crée un sous-total dans la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnNameRowIndex | int | L'index de ligne de la ligne de nom de colonne. |
| dataRows | int | Le nombre de lignes de données. |
| groupByColumnIndex | int | L'index de colonne de la colonne à regrouper. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Le type de fonction de sous-total. |
| subtotalColumnIndexList | int[] | Les index de colonnes à sous-totaliser. |
| functionLabel | java.lang.String | L'étiquette de la fonction de sous-total. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Le style de la ligne du total général. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Le style de la ligne de sous-total. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Le type numérique des cellules de résultat du sous-total. |
| customString | java.lang.String | La chaîne de format personnalisée des cellules de résultat du sous-total. Peut être nulle. |

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
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


Définit le filtre pour la colonne. Notez que nous devons appeler AddAutoFilter avant d'appeler filterString. La chaîne de critères du filtre. Notez que nous utilisons la virgule -> \",\" comme caractère de séparation, donc la valeur de cellule que vous souhaitez filtrer ne doit pas contenir de virgule. filterString(10,\"123,456\") signifie que la colonne 10 doit contenir 123 ou 456, filterString(10,\"123\") signifie que la colonne 10 doit contenir 123. L'index de colonne est séparé par des virgules, ex. 123,456,789 ou abc

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int |  |
| critères | java.lang.String |  |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Fige les volets à la cellule spécifiée dans la feuille de calcul.

**Remarks**

L'index de ligne et l'index de colonne ne peuvent pas tous les deux être zéro. Le nombre de lignes et le nombre de colonnes ne peuvent pas non plus être tous les deux zéro.

Les deux premiers paramètres spécifient la position gelée et les deux derniers paramètres spécifient la zone gelée dans le volet supérieur gauche.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| colonne | int | Indice de colonne. |
| freezedRows | int | Nombre de lignes visibles dans le volet supérieur, ne dépassant pas l'index de ligne. |
| freezedColumns | int | Nombre de colonnes visibles dans le volet gauche, ne dépassant pas l'index de colonne. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Fige les volets à la cellule spécifiée dans la feuille de calcul.

**Remarks**

L'index de ligne et l'index de colonne ne peuvent pas tous les deux être zéro. Le nombre de lignes et le nombre de colonnes ne peuvent pas non plus être tous les deux zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de cellule. |
| freezedRows | int | Nombre de lignes visibles dans le volet supérieur, ne dépassant pas l'index de ligne. |
| freezedColumns | int | Nombre de colonnes visibles dans le volet gauche, ne dépassant pas l'index de colonne. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Obtient la cellule active dans la feuille de calcul.

**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Obtient l'image d'arrière-plan de la feuille de calcul.

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```


Obtient la collection [GridCell](../../com.aspose.gridweb/gridcell).

**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Représente le nom de code de la feuille de calcul.

**Remarks**

Vous ne pouvez pas changer le nom du code tant que le fichier modèle contient VBA/macro.

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


Obtient la légende de la colonne. Si la légende n'est pas définie, renvoie une chaîne vide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |

**Returns:**
java.lang.String - La légende de la colonne. Si la légende n'est pas définie, renvoie une chaîne vide.
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


Obtient le texte de l'infobulle de l'en-tête de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colIndex | int | L'index de la colonne. |

**Returns:**
java.lang.String - Le texte de l'infobulle.
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


Obtient si une colonne est en lecture seule. Cette méthode étendue de GridWeb spécifiquement ne sera pas conservée ni prise en compte dans le fichier Excel réel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | indice de colonne. |

**Returns:**
boolean - Si en lecture seule, renvoie true.
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```


Obtient la collection [GridComment](../../com.aspose.gridweb/gridcomment).

**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. La valeur par défaut est false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


Vrai si les valeurs zéro sont affichées.

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Représente l'index de la première colonne visible.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Représente l'index de la première ligne visible.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Obtient les volets figés.

**Returns:**
int[] - Retourner null signifie que la feuille de calcul n'est pas figée 0:indice de ligne;1:colonne;2:lignes figées;3:lignes figées
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```


Obtient la cellule active dans la feuille de calcul.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


Obtient la collection [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection).

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtient l'index de la feuille dans la collection de feuilles de calcul.

**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


Obtient si la cellule est en lecture seule. Ceci est un attribut étendu de GridWeb, il ne sera pas conservé dans le fichier Excel réel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int |  |
| col | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la feuille de calcul.

**Remarks**

La longueur maximale du nom de feuille est de 31 caractères. Vous ne pouvez pas attribuer le même nom (insensible à la casse) à deux feuilles de calcul. Par exemple, vous ne pouvez pas définir \"SheetName1\" pour la première feuille et \"SHEETNAME1\" pour la seconde feuille.

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


Indique si l'affichage du contour est activé.

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


Obtient une collection [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--).

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


Obtient les tableaux croisés dynamiques dans la feuille de calcul.

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


Obtient la légende de la ligne. Si la légende n'est pas définie, renvoie une chaîne vide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |

**Returns:**
java.lang.String - La légende de la ligne. Si la légende n'est pas définie, renvoie une chaîne vide.
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


Obtient le texte de l'infobulle de l'en-tête de ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | L'index de la ligne. |

**Returns:**
java.lang.String - Le texte de l'infobulle.
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


Obtient si une ligne est readonly. c'est une méthode étendue de GridWeb spécifiquement, elle ne sera pas conservée et n'affectera pas le fichier Excel réel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | indice de ligne. |

**Returns:**
boolean - Si en lecture seule, renvoie true.
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert.

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


Obtient une collection [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--).

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
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
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Représente la couleur de l'onglet de la feuille de calcul.

**Remarks**

Cette fonctionnalité n'est prise en charge que dans ExcelXP (Excel2002) et les versions ultérieures. Si vous enregistrez le fichier au format Excel97 ou Excel2000, il sera omis.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Obtient l'UniqueID dans le Contrôle

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Obtient la collection des paramètres de validation des données dans la feuille de calcul.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Indique si le nom de cette feuille est affiché dans les onglets de feuilles du contrôle.

**Returns:**
boolean
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Obtient l'objet [GridWorkbook](../../com.aspose.gridweb/gridworkbook) de la collection de feuilles de calcul.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400.

**Returns:**
int
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
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Obtient une valeur indiquant si les lignes de grille sont visibles. La valeur par défaut est true.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indique si la feuille de calcul est protégée.

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


Indique si la ligne de résumé sera positionnée sous les lignes de détail dans le plan.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Déplace la feuille vers un autre emplacement dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | Index de la feuille de destination. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


Actualise les auto‑filtres pour masquer ou afficher les lignes.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Supprime le filtre automatique de la feuille de calcul.

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


Supprime le sous-total créé par la méthode CreateSubtotal dans la feuille.

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


Le décalage entier du champ sur lequel vous souhaitez appliquer, basé sur la première colonne de filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Définit la cellule active dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Rend toutes les cellules modifiables. Ceci est un attribut étendu.

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Rend toutes les cellules en lecture seule. Ceci est un attribut étendu, notez que cet attribut ne peut pas être conservé dans la cellule réelle ; si vous souhaitez conserver la protection, veuillez utiliser setProtect.

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Définit l'image d'arrière-plan de la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


Définit la légende pour la colonne. Veuillez noter que c'est un attribut d'extension et qu'il ne peut pas être conservé dans le fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |
| légende | java.lang.String | La légende de la colonne. Passez null ou une chaîne vide si vous voulez annuler la légende. |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


Définit le texte de l'infobulle de l'en-tête de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colIndex | int | L'index de la colonne. |
| info-bulle | java.lang.String | Le texte de l'info-bulle. |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


Définit une colonne en readonly afin que l'utilisateur ne puisse pas la supprimer côté client. c'est une méthode étendue de GridWeb spécifiquement, elle ne sera pas conservée et n'affectera pas le fichier Excel réel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | indice de colonne. |
| isReadonly | boolean | vrai ou faux. |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


Vrai si les valeurs zéro sont affichées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Rend une plage de cellules modifiable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendre toutes les cellules en lecture seule en appelant la méthode SetAllCellsReadonly. puis appelez cette méthode pour spécifier la plage de cellules qui doit être modifiable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ de la plage. |
| startColumn | int | La colonne de départ de la plage. |
| lignes | int | Le nombre de lignes. |
| colonnes | int | Le nombre de colonnes. |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Représente l'index de la première colonne visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Représente l'index de la première ligne visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


Définit la cellule active dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Définit une valeur indiquant si les lignes de grille sont visibles. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


Définit si la cellule est en lecture seule. Ceci est un attribut étendu de GridWeb, il ne sera pas conservé dans le fichier Excel réel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int |  |
| col | int |  |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la feuille de calcul.

**Remarks**

La longueur maximale du nom de feuille est de 31 caractères. Vous ne pouvez pas attribuer le même nom (insensible à la casse) à deux feuilles de calcul. Par exemple, vous ne pouvez pas définir \"SheetName1\" pour la première feuille et \"SHEETNAME1\" pour la seconde feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Indique si l'affichage du contour est activé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


Protège la feuille de calcul.

**Remarks**

Cette méthode protège la feuille de calcul sans mot de passe. Elle peut protéger la feuille de calcul dans toutes les versions du fichier Excel.

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Rend une plage de cellules en lecture seule. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Commencez par rendre toutes les cellules modifiables en appelant la méthode SetAllCellsEditable. puis appelez cette méthode pour spécifier la plage de cellules qui doit être en lecture seule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ de la plage. |
| startColumn | int | La colonne de départ de la plage. |
| lignes | int | Le nombre de lignes. |
| colonnes | int | Le nombre de colonnes. |

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


Définit la légende pour la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| légende | java.lang.String | La légende de la ligne. Passez null ou une chaîne vide si vous voulez annuler la légende. |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


Définit le texte de l'infobulle de l'en-tête de ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | L'index de la ligne. |
| info-bulle | java.lang.String | Le texte de l'info-bulle. |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


Définit une ligne en readonly afin que l'utilisateur ne puisse pas la supprimer côté client. c'est une méthode étendue de GridWeb spécifiquement, elle ne sera pas conservée et n'affectera pas le fichier Excel réel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | indice de ligne. |
| isReadonly | boolean | vrai ou faux. |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


Indique si la ligne de résumé sera positionnée sous les lignes de détail dans le plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


Représente la couleur de l'onglet de la feuille de calcul.

**Remarks**

Cette fonctionnalité n'est prise en charge que dans ExcelXP (Excel2002) et les versions ultérieures. Si vous enregistrez le fichier au format Excel97 ou Excel2000, il sera omis.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indique si le nom de cette feuille est affiché dans les onglets de feuilles du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Déverrouille les volets dans la feuille de calcul.

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


Dégroupe les lignes.

**Remarks**

Supprime uniquement les informations du groupe externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de ligne à dégrouper. |
| lastIndex | int | Le dernier indice de ligne à dégrouper. |

### unProtect() {#unProtect--}
```
public void unProtect()
```


Supprime la protection de la feuille de calcul.

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

