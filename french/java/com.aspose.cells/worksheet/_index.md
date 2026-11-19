---
title: "Worksheet"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente une seule feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

Encapsule l'objet qui représente une seule feuille de calcul.

**Example**

L’exemple suivant montre comment figer les volets et insérer un lien hypertexte dans la feuille de calcul avec .Net ou VB.

```
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | Ajoute un saut de page. |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | Filtre les données en utilisant des critères complexes. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Ajuste automatiquement la largeur de la colonne. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Ajuste automatiquement la largeur de la colonne. |
| [autoFitColumns()](#autoFitColumns--) | Ajuste automatiquement toutes les colonnes de cette feuille de calcul. |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | Ajuste automatiquement toutes les colonnes de cette feuille de calcul. |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | Ajuste automatiquement la largeur des colonnes. |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | Ajuste automatiquement la largeur des colonnes. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | Ajuste automatiquement la largeur des colonnes. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | Ajuste automatiquement la largeur des colonnes. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Ajuste automatiquement la hauteur de la ligne. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Ajuste automatiquement la hauteur de la ligne. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | Ajuste automatiquement la hauteur de la ligne. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Ajuste automatiquement la hauteur des lignes dans une plage rectangulaire. |
| [autoFitRows()](#autoFitRows--) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Ajuste automatiquement la hauteur des lignes dans une plage. |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | Ajuste automatiquement la hauteur des lignes dans une plage. |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Calcule une formule en tant que formule matricielle. |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | Calcule une formule en tant que formule matricielle. |
| [calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)](#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-) | Calcule une formule en tant que formule matricielle. |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | Calcule toutes les formules de cette feuille de calcul. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Calcule une formule. |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Calcule directement une expression de formule. |
| [calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)](#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-) | Calcule directement une expression de formule. |
| [clearComments()](#clearComments--) | Efface tous les commentaires dans la feuille de calcul du concepteur. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Ferme la session qui utilise des caches pour accéder aux données de cette feuille de calcul. |
| [convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)](#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-) | Convertit le style de référence de la formule. |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(CellArea ca)](#filter-com.aspose.cells.CellArea-) | Filtre la plage. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Fige les volets à la cellule spécifiée dans la feuille de calcul. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Fige les volets à la cellule spécifiée dans la feuille de calcul. |
| [getActiveCell()](#getActiveCell--) | Obtient la cellule active dans la feuille de calcul. |
| [getAdvancedFilter()](#getAdvancedFilter--) | Obtient les paramètres du filtre avancé. |
| [getAllPictures()](#getAllPictures--) | Récupère toutes les images, y compris celles intégrées dans la cellule et au-dessus des cellules. |
| [getAllowEditRanges()](#getAllowEditRanges--) | Obtient la collection des plages autorisées à l'édition dans la feuille de calcul. |
| [getAreasOfXmlMapQuery(String path, XmlMap xmlMap)](#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Interroge les zones de cellules qui sont mappées/liées au chemin spécifique de la carte XML. |
| [getAutoFilter()](#getAutoFilter--) | Représente le filtre automatique pour la feuille de calcul spécifiée. |
| [getBackgroundImage()](#getBackgroundImage--) | Obtient l'image d'arrière-plan de la feuille de calcul. |
| [getCellWatches()](#getCellWatches--) | Obtient la collection de cellules de cette feuille de calcul surveillée dans la 'fenêtre de surveillance'. |
| [getCells()](#getCells--) | Obtient la collection [Cells](../../com.aspose.cells/cells). |
| [getCharts()](#getCharts--) | Obtient une collection [Chart](../../com.aspose.cells/chart) |
| [getCheckBoxes()](#getCheckBoxes--) | Obtient une collection [CheckBox](../../com.aspose.cells/checkbox). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Obtient le nom de code de la feuille de calcul. |
| [getComments()](#getComments--) | Obtient la collection [Comment](../../com.aspose.cells/comment). |
| [getConditionalFormattings()](#getConditionalFormattings--) | Obtient les ConditionalFormattings dans la feuille de calcul. |
| [getCustomProperties()](#getCustomProperties--) | Obtient un objet représentant les informations d'identifiant associées à une feuille de calcul. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. |
| [getDisplayZeros()](#getDisplayZeros--) | Vrai si les valeurs zéro sont affichées. |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | Obtient le paramètre de vérification d'erreurs appliqué à certaines plages. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Représente l'index de la première colonne visible. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Représente l'index de la première ligne visible. |
| [getFreezedPanes()](#getFreezedPanes--) | Obtient les volets figés. |
| [getGridlineColor()](#getGridlineColor--) | Obtient la couleur de la ligne de grille |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Obtient la collection [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection). |
| [getHyperlinks()](#getHyperlinks--) | Obtient la collection [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection). |
| [getIndex()](#getIndex--) | Obtient l'index de la feuille dans la collection de feuilles de calcul. |
| [getListObjects()](#getListObjects--) | Obtient tous les ListObjects de cette feuille de calcul. |
| [getName()](#getName--) | Obtient le nom de la feuille de calcul. |
| [getOleObjects()](#getOleObjects--) | Représente une collection de [OleObject](../../com.aspose.cells/oleobject) dans une feuille de calcul. |
| [getOutline()](#getOutline--) | Obtient le contour de cette feuille de calcul. |
| [getPageSetup()](#getPageSetup--) | Représente la description de la mise en page de cette feuille. |
| [getPaneState()](#getPaneState--) | Indique si le volet possède des divisions horizontales ou verticales, et si ces divisions sont figées. |
| [getPanes()](#getPanes--) | Obtient les volets de la fenêtre. |
| [getPictures()](#getPictures--) | Obtient une collection de [Picture](../../com.aspose.cells/picture). |
| [getPivotTables()](#getPivotTables--) | Obtient tous les tableaux croisés dynamiques de cette feuille de calcul. |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | Obtient les sauts de page automatiques. |
| [getProtection()](#getProtection--) | Représente les différents types d'options de protection disponibles pour une feuille de calcul. |
| [getQueryTables()](#getQueryTables--) | Obtient le [QueryTableCollection](../../com.aspose.cells/querytablecollection) dans la feuille de calcul. |
| [getScenarios()](#getScenarios--) | Obtient la collection de [Scenario](../../com.aspose.cells/scenario). |
| [getSelectedAreas()](#getSelectedAreas--) | Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur. |
| [getSelectedRanges()](#getSelectedRanges--) | Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur. |
| [getShapes()](#getShapes--) | Renvoie toutes les formes de dessin de cette feuille de calcul. |
| [getShowDataTypeIcons()](#getShowDataTypeIcons--) | Indique s'il faut afficher les icônes de type de données. |
| [getShowFormulas()](#getShowFormulas--) | Indique s'il faut afficher les formules ou leurs résultats. |
| [getSlicers()](#getSlicers--) | Obtenez la collection de Slicer dans la feuille de calcul |
| [getSmartTagSetting()](#getSmartTagSetting--) | Obtient tous les objets [SmartTagCollection](../../com.aspose.cells/smarttagcollection) de la feuille de calcul. |
| [getSparklineGroups()](#getSparklineGroups--) | Obtient les groupes de sparkline dans la feuille de calcul. |
| [getTabColor()](#getTabColor--) | Représente la couleur de l'onglet de la feuille de calcul. |
| [getTabId()](#getTabId--) | Spécifie l'identifiant interne de la feuille. |
| [getTextBoxes()](#getTextBoxes--) | Obtient une collection de [TextBox](../../com.aspose.cells/textbox). |
| [getTimelines()](#getTimelines--) | Obtenez la collection de Timeline dans la feuille de calcul |
| [getTransitionEntry()](#getTransitionEntry--) | Indique si l'option Transition Formula Entry (compatibilité Lotus) est activée. |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | Indique si l'option Transition Formula Evaluation (compatibilité Lotus) est activée. |
| [getType()](#getType--) | Représente le type de feuille de calcul. |
| [getUniqueId()](#getUniqueId--) | Obtient l'identifiant unique, il est identique à \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [getValidations()](#getValidations--) | Obtient la collection des paramètres de validation des données dans la feuille de calcul. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | Obtient la collection [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection). |
| [getViewType()](#getViewType--) | Obtient le type de vue. |
| [getVisibilityType()](#getVisibilityType--) | Indique l'état de visibilité de cette feuille. |
| [getWorkbook()](#getWorkbook--) | Obtient l'objet classeur qui contient cette feuille. |
| [getZoom()](#getZoom--) | Représente le facteur d'échelle en pourcentage. |
| [hasAutofilter()](#hasAutofilter--) | Indique si cette feuille de calcul possède un filtre automatique. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Obtient une valeur indiquant si les lignes de quadrillage sont visibles. La valeur par défaut est vraie. |
| [isOutlineShown()](#isOutlineShown--) | Indique s'il faut afficher le contour. |
| [isPageBreakPreview()](#isPageBreakPreview--) | Indique si la feuille de calcul spécifiée est affichée en vue normale ou en aperçu des sauts de page. |
| [isProtected()](#isProtected--) | Indique si la feuille de calcul est protégée. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | Obtient une valeur indiquant si la feuille de calcul affichera les en-têtes de lignes et de colonnes. |
| [isRulerVisible()](#isRulerVisible--) | Indique si la règle est visible. |
| [isSelected()](#isSelected--) | Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert. |
| [isVisible()](#isVisible--) | Représente si la feuille de calcul est visible. |
| [moveTo(int index)](#moveTo-int-) | Déplace la feuille vers un autre emplacement dans la feuille de calcul. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | Protège la feuille de calcul. |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | Protège la feuille de calcul. |
| [refreshPivotTables()](#refreshPivotTables--) | Actualise tous les tableaux croisés dynamiques dans cette feuille de calcul. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Actualise tous les tableaux croisés dynamiques dans cette feuille de calcul. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | Supprime tous les objets de dessin dans cette feuille de calcul. |
| [removeAutoFilter()](#removeAutoFilter--) | Supprime le filtre automatique de la feuille de calcul. |
| [removeSplit()](#removeSplit--) | Supprime la fenêtre fractionnée. |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | Remplace le texte de toutes les cellules par une nouvelle chaîne. |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | Sélectionne une plage. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Définit la cellule active dans la feuille de calcul. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Définit l'image d'arrière-plan de la feuille de calcul. |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | Obtient le nom de code de la feuille de calcul. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Vrai si les valeurs zéro sont affichées. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Représente l'index de la première colonne visible. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Représente l'index de la première ligne visible. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Définit la couleur de la ligne de grille |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Définit une valeur indiquant si les lignes de quadrillage sont visibles. La valeur par défaut est vraie. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la feuille de calcul. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Indique s'il faut afficher le contour. |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | Indique si la feuille de calcul spécifiée est affichée en vue normale ou en aperçu des sauts de page. |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | Définit une valeur indiquant si la feuille de calcul affichera les en-têtes de lignes et de colonnes. |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | Indique si la règle est visible. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert. |
| [setShowDataTypeIcons(boolean value)](#setShowDataTypeIcons-boolean-) | Indique s'il faut afficher les icônes de type de données. |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | Indique s'il faut afficher les formules ou leurs résultats. |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | Représente la couleur de l'onglet de la feuille de calcul. |
| [setTabId(int value)](#setTabId-int-) | Spécifie l'identifiant interne de la feuille. |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | Indique si l'option Transition Formula Entry (compatibilité Lotus) est activée. |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | Indique si l'option Transition Formula Evaluation (compatibilité Lotus) est activée. |
| [setType(int value)](#setType-int-) | Représente le type de feuille de calcul. |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | Définit l'identifiant unique, il est identique à \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [setViewType(int value)](#setViewType-int-) | Définit le type de vue. |
| [setVisibilityType(int value)](#setVisibilityType-int-) | Indique l'état de visibilité de cette feuille. |
| [setVisible(boolean value)](#setVisible-boolean-) | Représente si la feuille de calcul est visible. |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | Définit les options visibles. |
| [setZoom(int value)](#setZoom-int-) | Représente le facteur d'échelle en pourcentage. |
| [split()](#split--) | Divise la fenêtre. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Démarre la session qui utilise le cache pour accéder aux données de cette feuille de calcul. |
| [toString()](#toString--) | Renvoie une chaîne qui représente l'objet Feuille de calcul actuel. |
| [unFreezePanes()](#unFreezePanes--) | Déverrouille les volets dans la feuille de calcul. |
| [unprotect()](#unprotect--) | Supprime la protection de la feuille de calcul. |
| [unprotect(String password)](#unprotect-java.lang.String-) | Supprime la protection de la feuille de calcul. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Interroge les zones de cellules qui sont mappées/liées au chemin spécifique de la carte XML. |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


Ajoute un saut de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


Filtre les données en utilisant des critères complexes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isFilter | boolean | Indique si le filtrage de la liste est effectué sur place. |
| listRange | java.lang.String | La plage de la liste. |
| criteriaRange | java.lang.String | La plage de critères. |
| copyTo | java.lang.String | La plage vers laquelle les données sont copiées. |
| uniqueRecordOnly | boolean | Affiche ou copie uniquement les lignes uniques. |

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


Ajuste automatiquement toutes les colonnes de cette feuille de calcul.

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


Ajuste automatiquement toutes les colonnes de cette feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Les options d'ajustement automatique |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


Ajuste automatiquement la largeur des colonnes.

**Remarks**

AutoFitColumn est une fonction imprécise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstColumn | int | Indice de la première colonne. |
| lastColumn | int | Dernier indice de colonne. |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


Ajuste automatiquement la largeur des colonnes.

**Remarks**

AutoFitColumn est une fonction imprécise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstColumn | int | Indice de la première colonne. |
| lastColumn | int | Dernier indice de colonne. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Les options d'ajustement automatique |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


Ajuste automatiquement la largeur des colonnes.

**Remarks**

AutoFitColumn est une fonction imprécise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Indice de la première ligne. |
| firstColumn | int | Indice de la première colonne. |
| lastRow | int | Indice de la dernière ligne. |
| lastColumn | int | Dernier indice de colonne. |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


Ajuste automatiquement la largeur des colonnes.

**Remarks**

AutoFitColumn est une fonction imprécise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Indice de la première ligne. |
| firstColumn | int | Indice de la première colonne. |
| lastRow | int | Indice de la dernière ligne. |
| lastColumn | int | Dernier indice de colonne. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Les options d'ajustement automatique |

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

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
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
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Les options de l'ajusteur automatique. |

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

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


Ajuste automatiquement toutes les lignes de cette feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Les options de l'ajusteur automatique. |

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

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


Ajuste automatiquement la hauteur des lignes dans une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| endRow | int | Indice de ligne de fin. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Les options de l'ajusteur automatique. |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


Calcule une formule en tant que formule matricielle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formule à calculer. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options pour calculer la formule |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


Calcule une formule en tant que formule matricielle.

**Remarks**

La formule sera considérée comme une formule de tableau dynamique pour calculer la dimension et le résultat. La dimension maximale spécifiée par l'utilisateur est utilisée dans les cas où le résultat calculé constitue un grand ensemble de données (par exemple, le résultat calculé peut correspondre à une ligne ou une colonne entière) mais l'utilisateur n'a pas besoin d'un tableau aussi grand selon les exigences métier ou pour des considérations de performance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formule à calculer. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options pour calculer la formule |
| maxRowCount | int | le nombre maximal de lignes des données résultantes. S'il est non positif ou supérieur au nombre réel de lignes, alors le nombre réel de lignes sera utilisé. |
| maxColumnCount | int | le nombre maximal de colonnes des données résultantes. S'il est non positif ou supérieur au nombre réel de lignes, alors le nombre réel de colonnes sera utilisé. |

**Returns:**
java.lang.Object[][] - Résultat de la formule calculée.
### calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData) {#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-}
```
public Object[][] calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)
```


Calcule une formule en tant que formule matricielle.

**Remarks**

La formule sera considérée comme une formule de tableau dynamique pour calculer la dimension et le résultat. La dimension maximale spécifiée par l'utilisateur est utilisée dans les cas où le résultat calculé constitue un grand ensemble de données (par exemple, le résultat calculé peut correspondre à une ligne ou une colonne entière) mais l'utilisateur n'a pas besoin d'un tableau aussi grand selon les exigences métier ou pour des considérations de performance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formule à calculer. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options pour analyser la formule |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options pour calculer la formule |
| baseCellRow | int | L'indice de ligne de la cellule de base. |
| baseCellColumn | int | L'indice de colonne de la cellule de base. |
| maxRowCount | int | Le nombre maximal de lignes des données résultantes. S'il est non positif ou supérieur au nombre réel de lignes, alors le nombre réel de lignes sera utilisé. |
| maxColumnCount | int | Le nombre maximal de colonnes des données résultantes. S'il est non positif ou supérieur au nombre réel de lignes, alors le nombre réel de colonnes sera utilisé. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Les données de calcul. Elles sont utilisées lorsqu'un utilisateur doit calculer des formules statiques lors de la mise en œuvre d'un moteur de calcul personnalisé. Pour ce type de situation, l'utilisateur doit les spécifier avec les données de calcul fournies pour [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object[][] - Résultat de la formule calculée.
### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


Calcule toutes les formules de cette feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options de calcul |
| recursive | boolean | True signifie que si les cellules de la feuille de calcul dépendent des cellules d'autres feuilles, les cellules dépendantes dans les autres feuilles seront également calculées. False signifie que toutes les formules de la feuille de calcul ont été calculées et que les valeurs sont correctes. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Calcule une formule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formule à calculer. |

**Returns:**
java.lang.Object - Résultat de la formule calculée.
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


Calcule directement une expression de formule.

**Remarks**

La formule sera calculée comme si elle avait été définie dans la cellule A1. Et la formule sera considérée comme une formule normale. Si vous avez besoin que la formule soit calculée comme une formule matricielle et d'obtenir un tableau pour le résultat calculé, veuillez utiliser [calculateArrayFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-CalculationOptions-) à la place.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formule à calculer. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options pour calculer la formule |

**Returns:**
java.lang.Object - Résultat calculé de la formule donnée. L'objet retourné peut être de types possibles tels que [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), ou ReferredArea.
### calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData) {#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-}
```
public Object calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)
```


Calcule directement une expression de formule.

**Remarks**

La formule sera calculée comme si elle avait été définie dans la cellule de base spécifiée. Et la formule sera considérée comme une formule normale. Si vous avez besoin que la formule soit calculée comme une formule matricielle et d'obtenir un tableau pour le résultat calculé, veuillez utiliser [calculateArrayFormula(String,FormulaParseOptions,CalculationOptions,int,int,int,int,CalculationData)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-FormulaParseOptions-CalculationOptions-int-int-int-int-CalculationData-) à la place.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | Formule à calculer. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options d'analyse de la formule. |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options de calcul de la formule. |
| baseCellRow | int | L'indice de ligne de la cellule de base. |
| baseCellColumn | int | L'indice de colonne de la cellule de base. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Les données de calcul. Elles sont utilisées lorsqu'un utilisateur doit calculer des formules statiques lors de la mise en œuvre d'un moteur de calcul personnalisé. Pour ce type de situation, l'utilisateur doit les spécifier avec les données de calcul fournies pour [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object - Résultat calculé de la formule donnée. L'objet retourné peut être de types possibles tels que [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), ou ReferredArea.
### clearComments() {#clearComments--}
```
public void clearComments()
```


Efface tous les commentaires dans la feuille de calcul du concepteur.

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Ferme la session qui utilise des caches pour accéder aux données de cette feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). options d'accès aux données |

### convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn) {#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-}
```
public String convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)
```


Convertit le style de référence de la formule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La formule à convertir. |
| toR1C1 | boolean | Quel style de référence utiliser pour convertir la formule. Si la formule originale est au style de référence A1, alors cette valeur doit être true afin que la formule soit convertie du style A1 au style R1C1 ; si la formule originale est au style de référence R1C1, alors cette valeur doit être false afin que la formule soit convertie du style R1C1 au style A1 ; |
| baseCellRow | int | L'indice de ligne de la cellule de base. |
| baseCellColumn | int | L'indice de colonne de la cellule de base. |

**Returns:**
java.lang.String - La formule convertie.
### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


Copie le contenu et les formats d'une autre feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Feuille de calcul source. |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


Copie le contenu et les formats d'une autre feuille de calcul.

**Remarks**

Vous pouvez copier des données d'une autre feuille de calcul dans le même fichier ou dans un autre fichier. Cependant, cette méthode ne prend pas en charge la copie d'objets graphiques, tels que les commentaires, les images et les graphiques.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Feuille de calcul source. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

### dispose() {#dispose--}
```
public void dispose()
```


Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées.

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
### filter(CellArea ca) {#filter-com.aspose.cells.CellArea-}
```
public void filter(CellArea ca)
```


Filtre la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage |

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
### getAdvancedFilter() {#getAdvancedFilter--}
```
public AdvancedFilter getAdvancedFilter()
```


Obtient les paramètres du filtre avancé.

**Returns:**
[AdvancedFilter](../../com.aspose.cells/advancedfilter) - 
### getAllPictures() {#getAllPictures--}
```
public Picture[] getAllPictures()
```


Récupère toutes les images, y compris celles intégrées dans la cellule et au-dessus des cellules.

**Returns:**
com.aspose.cells.Picture[] -
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


Obtient la collection des plages autorisées à l'édition dans la feuille de calcul.

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAreasOfXmlMapQuery(String path, XmlMap xmlMap) {#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public CellArea[] getAreasOfXmlMapQuery(String path, XmlMap xmlMap)
```


Interroge les zones de cellules qui sont mappées/liées au chemin spécifique de la carte XML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | java.lang.String | chemin de l'élément xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Spécifiez une carte xml si vous souhaitez interroger le chemin spécifique au sein d'une carte spécifique |

**Returns:**
com.aspose.cells.CellArea[] - liste [CellArea](../../com.aspose.cells/cellarea) qui est mappée/liée au chemin spécifique de la carte xml, une liste vide est renvoyée si rien n'est mappé/lié.
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Représente le filtre automatique pour la feuille de calcul spécifiée.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Obtient l'image d'arrière-plan de la feuille de calcul.

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


Obtient la collection de cellules de cette feuille de calcul surveillée dans la 'fenêtre de surveillance'.

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


Obtient la collection [Cells](../../com.aspose.cells/cells).

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


Obtient une collection [Chart](../../com.aspose.cells/chart)

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


Obtient une collection [CheckBox](../../com.aspose.cells/checkbox).

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
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


Obtient le nom de code de la feuille de calcul.

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


Obtient la collection [Comment](../../com.aspose.cells/comment).

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


Obtient les ConditionalFormattings dans la feuille de calcul.

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


Obtient un objet représentant les informations d'identifiant associées à une feuille de calcul.

**Remarks**

Worksheet.CustomProperties offre un mécanisme privilégié pour stocker des données arbitraires. Il prend en charge les composants de documents tiers hérités, ainsi que les situations nécessitant strictement des parties binaires.

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
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
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


Obtient le paramètre de vérification d'erreurs appliqué à certaines plages.

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
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
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Obtient la couleur de la ligne de grille

**Returns:**
[Color](../../com.aspose.cells/color)
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


Obtient la collection [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection).

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


Obtient la collection [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection).

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtient l'index de la feuille dans la collection de feuilles de calcul.

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


Obtient tous les ListObjects de cette feuille de calcul.

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la feuille de calcul.

**Remarks**

La longueur maximale du nom de feuille est de 31 caractères. Vous ne pouvez pas attribuer le même nom (insensible à la casse) à deux feuilles de calcul. Par exemple, vous ne pouvez pas définir \"SheetName1\" pour la première feuille et \"SHEETNAME1\" pour la seconde feuille.

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


Représente une collection de [OleObject](../../com.aspose.cells/oleobject) dans une feuille de calcul.

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


Obtient le contour de cette feuille de calcul.

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Représente la description de la mise en page de cette feuille.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


Indique si le volet possède des divisions horizontales ou verticales, et si ces divisions sont figées.

Voir [PaneStateType](../../com.aspose.cells/panestatetype).

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


Obtient les volets de la fenêtre.

**Remarks**

Si la fenêtre n'est pas divisée ou figée.

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


Obtient une collection de [Picture](../../com.aspose.cells/picture).

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


Obtient tous les tableaux croisés dynamiques de cette feuille de calcul.

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


Obtient les sauts de page automatiques.

**Remarks**

Chaque zone de cellule représente une page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Les options d'impression |

**Returns:**
com.aspose.cells.CellArea[] - Les zones de sauts de page automatiques.
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


Représente les différents types d'options de protection disponibles pour une feuille de calcul. Prend en charge les options de protection avancées dans ExcelXP et les versions ultérieures.

**Remarks**

Cette propriété peut protéger la feuille de calcul dans toutes les versions de fichiers Excel et prendre en charge les options de protection avancées dans ExcelXP et les versions ultérieures.

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


Obtient le [QueryTableCollection](../../com.aspose.cells/querytablecollection) dans la feuille de calcul.

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


Obtient la collection de [Scenario](../../com.aspose.cells/scenario).

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedAreas() {#getSelectedAreas--}
```
public Range[] getSelectedAreas()
```


Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur.

**Returns:**
com.aspose.cells.Range[] - Retourne toutes les plages sélectionnées.
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser la méthode Worksheet.GetSelectedAreas(). Cette propriété sera supprimée 12 mois plus tard à compter de mars 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
java.util.ArrayList - Une ArrayList qui contient les plages sélectionnées.
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Renvoie toutes les formes de dessin de cette feuille de calcul.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTypeIcons() {#getShowDataTypeIcons--}
```
public boolean getShowDataTypeIcons()
```


Indique s'il faut afficher les icônes de type de données.

**Returns:**
boolean
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


Indique s'il faut afficher les formules ou leurs résultats.

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


Obtenez la collection de Slicer dans la feuille de calcul

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


Obtient tous les objets [SmartTagCollection](../../com.aspose.cells/smarttagcollection) de la feuille de calcul.

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


Obtient les groupes de sparkline dans la feuille de calcul.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Représente la couleur de l'onglet de la feuille de calcul.

**Remarks**

Cette fonctionnalité n'est prise en charge que dans ExcelXP (Excel2002) et les versions ultérieures. Si vous enregistrez le fichier au format Excel97 ou Excel2000, elle sera omise.

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


Spécifie l'identifiant interne de la feuille.

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


Obtient une collection de [TextBox](../../com.aspose.cells/textbox).

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


Obtenez la collection de Timeline dans la feuille de calcul

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


Indique si l'option Transition Formula Entry (compatibilité Lotus) est activée.

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


Indique si l'option Transition Formula Evaluation (compatibilité Lotus) est activée.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Représente le type de feuille de calcul.

Voir [SheetType](../../com.aspose.cells/sheettype).

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


Obtient l'identifiant unique, il est identique à \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


Obtient la collection des paramètres de validation des données dans la feuille de calcul.

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


Obtient la collection [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection).

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


Obtient le type de vue.

Voir [ViewType](../../com.aspose.cells/viewtype).

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


Indique l'état de visibilité de cette feuille.

Voir [VisibilityType](../../com.aspose.cells/visibilitytype).

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtient l'objet classeur qui contient cette feuille.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400.

**Remarks**

Veuillez d'abord définir le type de vue.

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


Indique si cette feuille de calcul possède un filtre automatique.

**Returns:**
boolean
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


Obtient une valeur indiquant si les lignes de quadrillage sont visibles. La valeur par défaut est vraie.

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


Indique s'il faut afficher le contour.

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


Indique si la feuille de calcul spécifiée est affichée en vue normale ou en aperçu des sauts de page.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indique si la feuille de calcul est protégée.

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


Obtient une valeur indiquant si la feuille de calcul affichera les en-têtes de lignes et de colonnes. La valeur par défaut est true.

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


Indique si la règle est visible. Cette propriété n'est appliquée que pour l'aperçu des sauts de page.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Représente si la feuille de calcul est visible.

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




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


Protège la feuille de calcul.

**Remarks**

Cette méthode protège la feuille de calcul sans mot de passe. Elle peut protéger la feuille de calcul dans toutes les versions du fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Type de protection. |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


Protège la feuille de calcul.

**Remarks**

Cette méthode peut protéger la feuille de calcul dans toutes les versions du fichier Excel.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Type de protection. |
| password | java.lang.String | Mot de passe. |
| oldPassword | java.lang.String | Si la feuille de calcul est déjà protégée par un mot de passe, veuillez fournir l'ancien mot de passe. Sinon, vous pouvez définir une valeur nulle ou une chaîne vide pour ce paramètre. |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Actualise tous les tableaux croisés dynamiques dans cette feuille de calcul.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Actualise tous les tableaux croisés dynamiques dans cette feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | L'option de rafraîchissement de la source de données du tableau croisé dynamique. |

**Returns:**
boolean
### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


Supprime tous les objets de dessin dans cette feuille de calcul.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Supprime le filtre automatique de la feuille de calcul.

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


Supprime la fenêtre fractionnée.

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


Remplace le texte de toutes les cellules par une nouvelle chaîne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldString | java.lang.String | Valeur de chaîne ancienne. |
| newString | java.lang.String | Valeur de chaîne nouvelle. |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


Sélectionne une plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ. |
| startColumn | int | La colonne de départ |
| totalRows | int | Le nombre de lignes. |
| totalColumns | int | Le nombre de colonnes |
| removeOthers | boolean | True signifie que les autres plages sélectionnées sont supprimées et que seule cette plage est sélectionnée. |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Définit la cellule active dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Définit l'image d'arrière-plan de la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


Obtient le nom de code de la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Définit la couleur de la ligne de grille

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Définit une valeur indiquant si les lignes de quadrillage sont visibles. La valeur par défaut est vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
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


Indique s'il faut afficher le contour.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


Indique si la feuille de calcul spécifiée est affichée en vue normale ou en aperçu des sauts de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


Définit une valeur indiquant si la feuille de calcul affichera les en-têtes de lignes et de colonnes. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


Indique si la règle est visible. Cette propriété n'est appliquée que pour l'aperçu des sauts de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowDataTypeIcons(boolean value) {#setShowDataTypeIcons-boolean-}
```
public void setShowDataTypeIcons(boolean value)
```


Indique s'il faut afficher les icônes de type de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


Indique s'il faut afficher les formules ou leurs résultats.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


Représente la couleur de l'onglet de la feuille de calcul.

**Remarks**

Cette fonctionnalité n'est prise en charge que dans ExcelXP (Excel2002) et les versions ultérieures. Si vous enregistrez le fichier au format Excel97 ou Excel2000, elle sera omise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


Spécifie l'identifiant interne de la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


Indique si l'option Transition Formula Entry (compatibilité Lotus) est activée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


Indique si l'option Transition Formula Evaluation (compatibilité Lotus) est activée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Représente le type de feuille de calcul.

Voir [SheetType](../../com.aspose.cells/sheettype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


Définit l'identifiant unique, il est identique à \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


Définit le type de vue.

Voir [ViewType](../../com.aspose.cells/viewtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


Indique l'état de visibilité de cette feuille.

Voir [VisibilityType](../../com.aspose.cells/visibilitytype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Représente si la feuille de calcul est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


Définit les options visibles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isVisible | boolean | Si la feuille de calcul est visible |
| ignoreError | boolean | Indique s'il faut ignorer l'erreur si cette option n'est pas valide. |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400.

**Remarks**

Veuillez d'abord définir le type de vue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### split() {#split--}
```
public void split()
```


Divise la fenêtre.

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Démarre la session qui utilise le cache pour accéder aux données de cette feuille de calcul.

**Remarks**

Après avoir terminé l'accès aux données, [closeAccessCache(int)](../../com.aspose.cells/worksheet\#closeAccessCache-int-) doit être invoqué avec les mêmes options pour effacer tous les caches et rétablir le mode d'accès normal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). options d'accès aux données |

### toString() {#toString--}
```
public String toString()
```


Renvoie une chaîne qui représente l'objet Feuille de calcul actuel.

**Returns:**
java.lang.String -
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Déverrouille les volets dans la feuille de calcul.

### unprotect() {#unprotect--}
```
public void unprotect()
```


Supprime la protection de la feuille de calcul.

**Remarks**

Cette méthode désactive la protection de la feuille de calcul qui est protégée sans mot de passe.

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Supprime la protection de la feuille de calcul.

**Remarks**

Si la feuille de calcul est protégée sans mot de passe, vous pouvez définir une valeur null ou une chaîne vide pour le paramètre password.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Mot de passe |

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

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


Interroge les zones de cellules qui sont mappées/liées au chemin spécifique de la carte XML.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Worksheet.GetAreasOfXmlMapQuery(). Cette propriété sera supprimée 12 mois plus tard à compter d'août 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | java.lang.String | chemin de l'élément xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Spécifiez une carte xml si vous souhaitez interroger le chemin spécifique au sein d'une carte spécifique |

**Returns:**
java.util.ArrayList - [CellArea](../../com.aspose.cells/cellarea) liste qui est mappée/liée au chemin spécifique de la carte XML, une liste vide est renvoyée si rien n'est mappé/lié.
