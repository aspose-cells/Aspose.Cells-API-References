---
title: "Tableau croisé dynamique"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Description résumée pour PivotTable."
type: docs
url: /fr/java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

Description résumée pour PivotTable.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
          PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
          calculateOption.setRefreshData(true);
          calculateOption.setRefreshCharts(true);
          pivot.calculateData(calculateOption); 
 
         //do your business
 
         book.save("out.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | Ajoute un champ calculé au champ pivot et le fait glisser vers la zone de données. |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | Ajoute un champ calculé au champ pivot. |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | Ajoute le champ à la zone spécifique. |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Ajoute le champ à la zone spécifique. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Ajoute le champ à la zone spécifique. |
| [calculateData()](#calculateData--) | Calcule les données du tableau croisé dynamique vers les cellules. |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | Calcule le tableau croisé dynamique avec des options. |
| [calculateRange()](#calculateRange--) | Calcule la plage du tableau croisé dynamique. |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | Modifie la source de données du tableau croisé dynamique. |
| [clearAll()](#clearAll--) | Supprime tous les champs des régions. |
| [clearData()](#clearData--) | Efface les données et le formatage de la vue du tableau croisé dynamique. |
| [clearFilters()](#clearFilters--) | Efface tous les filtres de ce tableau croisé dynamique. |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | Copie le style nommé d'un autre tableau croisé dynamique. |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportViewToJson(PivotViewToJsonOptions options)](#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-) | Exporte la vue du tableau croisé dynamique au format JSON. |
| [fields(int fieldType)](#fields-int-) | Obtient les champs spécifiques par type de champ. |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Formate la zone sélectionnée du tableau croisé dynamique. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Formate la zone sélectionnée du tableau croisé dynamique. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Formate la cellule dans la zone du tableau croisé dynamique |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | Formate toutes les cellules dans la zone du tableau croisé dynamique |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | Formate les données de ligne dans la zone du tableau croisé dynamique |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [getAltTextDescription()](#getAltTextDescription--) | Obtient la description du texte alternatif. |
| [getAltTextTitle()](#getAltTextTitle--) | Obtient le titre du texte alternatif. |
| [getAutoFormatType()](#getAutoFormatType--) | Obtient le type de formatage automatique du tableau croisé dynamique. |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | Indique s'il faut ajuster automatiquement la largeur des colonnes lors de la mise à jour |
| [getBaseFields()](#getBaseFields--) | Renvoie tous les champs de base du tableau croisé dynamique. |
| [getButtonArea(int axisType)](#getButtonArea-int-) | Obtient la zone contenant le bouton de champ. |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | Obtient l'objet [Cell](../../com.aspose.cells/cell) par le nom d'affichage du PivotField. |
| [getChildren()](#getChildren--) | Obtient les tableaux croisés dynamiques enfants qui utilisent les données de ce tableau croisé dynamique comme source de données. |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | Renvoie un objet PivotFields qui est actuellement affiché comme champs de colonne. |
| [getColumnGrand()](#getColumnGrand--) | Indique si le rapport du tableau croisé dynamique affiche les totaux généraux pour les colonnes. |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | Obtient la légende personnalisée de l'en-tête de colonne du tableau croisé dynamique. |
| [getColumnRange()](#getColumnRange--) | Renvoie un objet CellArea qui représente la plage contenant la zone de colonne dans le rapport du tableau croisé dynamique. |
| [getConditionalFormats()](#getConditionalFormats--) | Obtient les formats conditionnels du tableau croisé dynamique. |
| [getCustomListSort()](#getCustomListSort--) | Indique s'il faut prendre en compte la liste personnalisée intégrée lors du tri des données |
| [getDataBodyRange()](#getDataBodyRange--) | Renvoie un objet [CellArea](../../com.aspose.cells/cellarea) qui représente la plage contenant la zone de données dans la liste entre la ligne d'en-tête et la ligne d'insertion. |
| [getDataField()](#getDataField--) | Obtient un objet [PivotField](../../com.aspose.cells/pivotfield) qui représente tous les champs de données d'un tableau croisé dynamique. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | Obtient le nom de l’en-tête du champ de la zone de valeurs dans le tableau croisé dynamique. |
| [getDataFields()](#getDataFields--) | Obtient une [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) qui représente tous les champs de données d’un tableau croisé dynamique. |
| [getDataSource()](#getDataSource--) | Obtient la source de données du tableau croisé dynamique. |
| [getDependentPivotTables()](#getDependentPivotTables--) | Obtient tous les [PivotTable](../../com.aspose.cells/pivottable)s qui utilisent ce tableau croisé dynamique comme source de données. |
| [getDisplayErrorString()](#getDisplayErrorString--) | Indique si le rapport du tableau croisé dynamique affiche une chaîne personnalisée dans les cellules contenant des erreurs. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | Indique si les éléments des zones de lignes et de colonnes sont visibles lorsque la zone de données du tableau croisé dynamique est vide. |
| [getDisplayNullString()](#getDisplayNullString--) | Indique si le rapport du tableau croisé dynamique affiche une chaîne personnalisée si la valeur est nulle. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | Spécifie une valeur booléenne qui indique si l’utilisateur est autorisé à modifier les cellules de la zone de données du tableau croisé dynamique. |
| [getEnableDrilldown()](#getEnableDrilldown--) | Indique si le drilldown est activé. |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | Indique si la boîte de dialogue Champ du tableau croisé dynamique est disponible lorsque l’utilisateur double-clique sur le champ du tableau croisé dynamique. |
| [getEnableFieldList()](#getEnableFieldList--) | Indique si la liste des champs du tableau croisé dynamique est disponible dans la vue d’Excel. |
| [getEnableWizard()](#getEnableWizard--) | Indique si l’assistant Tableau croisé dynamique est disponible. |
| [getErrorString()](#getErrorString--) | Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | Obtient la source de données de connexion externe. |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | Indique si les champs du tableau croisé dynamique sont triés dans un ordre non par défaut dans la liste des champs. |
| [getFields(int fieldType)](#getFields-int-) | Obtient la liste de champs pivot spécifique par région. |
| [getFilterArea()](#getFilterArea--) | Obtient la zone de la région de filtre. |
| [getGrandTotalName()](#getGrandTotalName--) | Renvoie l’étiquette affichée dans l’en-tête de colonne ou de ligne du total général. |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | Obtient la liste des index de lignes du tableau croisé dynamique des sauts de page horizontaux. |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Obtient les sauts de page horizontaux de ce tableau croisé dynamique. |
| [getIndent()](#getIndent--) | Spécifie l’incrément d’indentation pour l’axe compact et peut être utilisé pour définir la mise en page du rapport en forme compacte. |
| [getItemPrintTitles()](#getItemPrintTitles--) | Indique si les noms de PivotItem doivent être répétés en haut de chaque page imprimée. |
| [getManualUpdate()](#getManualUpdate--) | Indique si le rapport du tableau croisé dynamique est recalculé uniquement à la demande de l’utilisateur. |
| [getMergeLabels()](#getMergeLabels--) | Obtient s’il faut fusionner les étiquettes de champs ligne/colonne qui s’étendent sur plusieurs cellules. |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [getName()](#getName--) | Obtient le nom du tableau croisé dynamique |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | Obtient les noms des connexions de données source externes. |
| [getNullString()](#getNullString--) | Obtient la chaîne affichée dans les cellules contenant des valeurs nulles lorsque la propriété DisplayNullString est vraie. La valeur par défaut est une chaîne vide. |
| [getPageFieldOrder()](#getPageFieldOrder--) | Obtient l'ordre dans lequel les champs de page sont ajoutés à la disposition du rapport de tableau croisé dynamique. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport de tableau croisé dynamique. |
| [getPageFields()](#getPageFields--) | Renvoie une [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) qui sont actuellement affichées en tant que champs de page. |
| [getPivotCache()](#getPivotCache--) | Obtient la source de données. |
| [getPivotFilters()](#getPivotFilters--) | Renvoie tous les filtres du tableau croisé dynamique. |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | Obtient les conditions de format du tableau croisé dynamique. |
| [getPivotFormats()](#getPivotFormats--) | Obtient tous les formats de cellule appliqués à ce tableau croisé dynamique. |
| [getPivotTableStyle()](#getPivotTableStyle--) | Obtient les paramètres de [TableStyle](../../com.aspose.cells/tablestyle) de ce tableau croisé dynamique. |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | Obtient le nom du style du tableau croisé dynamique. |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | Obtient le style intégré du tableau croisé dynamique. |
| [getPivotTablesWithSamePivotCache()](#getPivotTablesWithSamePivotCache--) | Obtient tous les tableaux croisés dynamiques partageant le même cache de tableau croisé dynamique. |
| [getPreserveCellFormattingOnUpdate()](#getPreserveCellFormattingOnUpdate--) | Indique s'il faut préserver le format des cellules ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) lorsque le tableau croisé dynamique est actualisé ou recalculé. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Indique si le format des cellules ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) est préservé lorsque le tableau croisé dynamique est actualisé ou recalculé. |
| [getPrintDrill()](#getPrintDrill--) | Spécifie une valeur booléenne indiquant si les indicateurs de forage doivent être imprimés. |
| [getPrintTitles()](#getPrintTitles--) | Indique si les titres d'impression de la feuille de calcul sont définis en fonction du rapport de tableau croisé dynamique. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | Indique si l'option Refresh Data est activée lors de l'ouverture du fichier. |
| [getRefreshDate()](#getRefreshDate--) | Obtient la date et l'heure de la dernière actualisation du tableau croisé dynamique. |
| [getRefreshedByWho()](#getRefreshedByWho--) | Obtient le nom du dernier utilisateur qui a actualisé ce tableau croisé dynamique. |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | Indique si les légendes des éléments de tableau croisé dynamique dans la zone de lignes sont répétées sur chaque page imprimée pour les champs de tableau croisé dynamique sous forme tabulaire. |
| [getRowFields()](#getRowFields--) | Renvoie une [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) qui sont actuellement affichées en tant que champs de ligne. |
| [getRowGrand()](#getRowGrand--) | Indique s'il faut afficher les totaux généraux pour les lignes de ce tableau croisé dynamique. |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | Obtient la légende personnalisée de l'en-tête de ligne dans ce tableau croisé dynamique. |
| [getRowRange()](#getRowRange--) | Renvoie un objet CellArea qui représente la plage contenant la zone de lignes dans le rapport de tableau croisé dynamique. |
| [getSaveData()](#getSaveData--) | Indique si les données du rapport de tableau croisé dynamique sont enregistrées avec le classeur. |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | Indique s'il faut afficher les totaux généraux pour les colonnes de ce tableau croisé dynamique. |
| [getShowDataTips()](#getShowDataTips--) | Indique si les infobulles doivent être affichées pour les cellules de données du tableau croisé dynamique. |
| [getShowDrill()](#getShowDrill--) | Obtient si l'affichage des boutons d'expansion/réduction est activé. |
| [getShowEmptyCol()](#getShowEmptyCol--) | Indique s'il faut inclure les colonnes vides dans le tableau. |
| [getShowEmptyRow()](#getShowEmptyRow--) | Indique s'il faut inclure les lignes vides dans le tableau. |
| [getShowHeaders()](#getShowHeaders--) | Indique s'il faut afficher les légendes des champs de données et les légendes des champs de tableau croisé dynamique sur l'axe des lignes et l'axe des colonnes dans la vue du tableau croisé dynamique. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | Spécifie une valeur booléenne indiquant si les informations de propriété des membres doivent être omises des infobulles du tableau croisé dynamique. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | Indique si l'en-tête de colonne du tableau croisé dynamique doit recevoir le style appliqué. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | Indique si le formatage en bandes est appliqué aux colonnes. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | Indique si le formatage de la colonne est appliqué. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | Indique si l'en-tête de ligne du tableau croisé dynamique doit recevoir le style appliqué. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | Indique si le formatage en bandes des lignes est appliqué. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | Indique s'il faut afficher les totaux généraux pour les lignes du tableau croisé dynamique. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | Indique si la légende de l'en-tête de ligne est affichée dans le rapport du tableau croisé dynamique. Indique si les légendes des champs d'affichage et les listes déroulantes de filtre sont affichées. |
| [getShowValuesRow()](#getShowValuesRow--) | Indique si la ligne des valeurs est affichée. |
| [getSource()](#getSource--) | Obtient la source de données de ce tableau croisé dynamique. |
| [getSource(boolean isOriginal)](#getSource-boolean-) | Obtient la source de données de ce tableau croisé dynamique. |
| [getSourceDataConnections()](#getSourceDataConnections--) | Obtient les sources de données de connexion externes. |
| [getSourceType()](#getSourceType--) | Obtient le type de source de données du tableau croisé dynamique. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | Indique si les éléments de champ de page masqués dans le rapport du tableau croisé dynamique sont inclus dans les sous-totaux des lignes et des colonnes, les totaux de bloc et les totaux généraux. |
| [getTableRange1()](#getTableRange1--) | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport du tableau croisé dynamique, mais n'inclut pas les champs de page. |
| [getTableRange2()](#getTableRange2--) | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport du tableau croisé dynamique, incluant les champs de page. |
| [getTag()](#getTag--) | Obtient une chaîne définie par l'utilisateur associée à cette vue du tableau croisé dynamique. |
| [getTopRightArea()](#getTopRightArea--) | Représente la zone vide en haut à droite du tableau croisé dynamique (en haut à gauche pour les feuilles RTL). |
| [getValuesField()](#getValuesField--) | Obtient un objet [PivotField](../../com.aspose.cells/pivotfield) qui représente tous les champs de données d'un tableau croisé dynamique. |
| [hasBlankRows()](#hasBlankRows--) | Indique s'il faut ajouter des lignes vides. |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | Indique si le rapport PivotTable est formaté automatiquement. |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | Spécifie si le PivotTable est compatible avec Excel2003 lors du rafraîchissement du PivotTable ; si vrai, une chaîne doit contenir au maximum 255 caractères, donc si la chaîne dépasse 255 caractères, elle sera tronquée. Si faux, une chaîne n’aura pas la restriction susmentionnée. |
| [isGridDropZones()](#isGridDropZones--) | Indique si le rapport PivotTable affiche la mise en page classique. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [isSelected()](#isSelected--) | Indique si ce PivotTable est sélectionné. |
| [move(int row, int column)](#move-int-int-) | Déplace le PivotTable vers un autre emplacement dans la feuille de calcul. |
| [move(String destCellName)](#move-java.lang.String-) | Déplace le PivotTable vers un autre emplacement dans la feuille de calcul. |
| [moveItem(int region, String[] nodes, boolean absolute, int offset)](#moveItem-int-java.lang.String---boolean-int-) | Déplace un élément vers le haut ou vers le bas. |
| [moveTo(int row, int column)](#moveTo-int-int-) | Déplace le PivotTable vers un autre emplacement dans la feuille de calcul. |
| [moveTo(int sheetIndex, int row, int column)](#moveTo-int-int-int-) | Déplace le PivotTable vers un autre emplacement dans la feuille de calcul. |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | Déplace le PivotTable vers un autre emplacement dans la feuille de calcul. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Actualise [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) depuis la source de données et calcule les données et le style pour la vue du pivot. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Actualise [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) depuis la source de données et calcule les données et le style pour la vue du pivot. |
| [refreshData()](#refreshData--) | Actualise les données depuis sa source de données vers le cache du pivot. |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | Actualise les données et les paramètres du PivotTable depuis sa source de données avec des options. |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | Supprimer le champ d'une zone de champ spécifique |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | Supprime un champ d'une région de pivot spécifique. |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | Supprime un champ d'une zone de champ spécifique. |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | Sélectionner une zone de la vue du tableau croisé dynamique. |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | Obtient la description du texte alternatif. |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | Définit le titre du texte alternatif. |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | Indique si le rapport PivotTable est formaté automatiquement. |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | Définit le type de format automatique du PivotTable. |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | Indique s'il faut ajuster automatiquement la largeur des colonnes lors de la mise à jour |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | Indique si le rapport du tableau croisé dynamique affiche les totaux généraux pour les colonnes. |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | Définit la légende personnalisée de l'en-tête de colonne du PivotTable. |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | Indique s'il faut prendre en compte la liste personnalisée intégrée lors du tri des données |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | Définit le nom de l'en-tête du champ de la zone de valeurs dans le PivotTable. |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | Définit la source de données du tableau croisé dynamique. |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | Indique si le rapport du tableau croisé dynamique affiche une chaîne personnalisée dans les cellules contenant des erreurs. |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | Indique si les éléments des zones de lignes et de colonnes sont visibles lorsque la zone de données du tableau croisé dynamique est vide. |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | Indique si le rapport du tableau croisé dynamique affiche une chaîne personnalisée si la valeur est nulle. |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | Spécifie une valeur booléenne qui indique si l’utilisateur est autorisé à modifier les cellules de la zone de données du tableau croisé dynamique. |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | Indique si le drilldown est activé. |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | Indique si la boîte de dialogue Champ du tableau croisé dynamique est disponible lorsque l’utilisateur double-clique sur le champ du tableau croisé dynamique. |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | Indique si la liste des champs du tableau croisé dynamique est disponible dans la vue d’Excel. |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | Indique si l’assistant Tableau croisé dynamique est disponible. |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide. |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | Spécifie si le PivotTable est compatible avec Excel2003 lors du rafraîchissement du PivotTable ; si vrai, une chaîne doit contenir au maximum 255 caractères, donc si la chaîne dépasse 255 caractères, elle sera tronquée. Si faux, une chaîne n’aura pas la restriction susmentionnée. |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | Indique si les champs du tableau croisé dynamique sont triés dans un ordre non par défaut dans la liste des champs. |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | Renvoie l’étiquette affichée dans l’en-tête de colonne ou de ligne du total général. |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | Indique si le rapport PivotTable affiche la mise en page classique. |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | Indique s'il faut ajouter des lignes vides. |
| [setIndent(int value)](#setIndent-int-) | Spécifie l’incrément d’indentation pour l’axe compact et peut être utilisé pour définir la mise en page du rapport en forme compacte. |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | Indique si les noms de PivotItem doivent être répétés en haut de chaque page imprimée. |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | Indique si le rapport du tableau croisé dynamique est recalculé uniquement à la demande de l’utilisateur. |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | Définit s'il faut fusionner les libellés de champs ligne/colonne qui s'étendent sur plusieurs cellules. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [setName(String value)](#setName-java.lang.String-) | Obtient le nom du tableau croisé dynamique |
| [setNullString(String value)](#setNullString-java.lang.String-) | Obtient la chaîne affichée dans les cellules contenant des valeurs nulles lorsque la propriété DisplayNullString est vraie. La valeur par défaut est une chaîne vide. |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | Définit l'ordre dans lequel les champs de page sont ajoutés à la mise en page du rapport PivotTable. |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport de tableau croisé dynamique. |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | Obtient les paramètres de [TableStyle](../../com.aspose.cells/tablestyle) de ce tableau croisé dynamique. |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | Définit le nom du style du tableau croisé dynamique. |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | Définit le style intégré du tableau croisé dynamique. |
| [setPreserveCellFormattingOnUpdate(boolean value)](#setPreserveCellFormattingOnUpdate-boolean-) | Indique s'il faut préserver le format des cellules ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) lorsque le tableau croisé dynamique est actualisé ou recalculé. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Indique si le format des cellules ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) est préservé lorsque le tableau croisé dynamique est actualisé ou recalculé. |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | Spécifie une valeur booléenne indiquant si les indicateurs de forage doivent être imprimés. |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | Indique si les titres d'impression de la feuille de calcul sont définis en fonction du rapport de tableau croisé dynamique. |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | Indique si l'option Refresh Data est activée lors de l'ouverture du fichier. |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | Indique si les légendes des éléments de tableau croisé dynamique dans la zone de lignes sont répétées sur chaque page imprimée pour les champs de tableau croisé dynamique sous forme tabulaire. |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | Indique s'il faut afficher les totaux généraux pour les lignes de ce tableau croisé dynamique. |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | Définit la légende personnalisée de l'en-tête de ligne dans ce PivotTable. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Indique si les données du rapport de tableau croisé dynamique sont enregistrées avec le classeur. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indique si ce PivotTable est sélectionné. |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | Indique s'il faut afficher les totaux généraux pour les colonnes de ce tableau croisé dynamique. |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | Indique si les infobulles doivent être affichées pour les cellules de données du tableau croisé dynamique. |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | Définit s'il faut afficher les boutons d'extension/réduction. |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | Indique s'il faut inclure les colonnes vides dans le tableau. |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | Indique s'il faut inclure les lignes vides dans le tableau. |
| [setShowHeaders(boolean value)](#setShowHeaders-boolean-) | Indique s'il faut afficher les légendes des champs de données et les légendes des champs de tableau croisé dynamique sur l'axe des lignes et l'axe des colonnes dans la vue du tableau croisé dynamique. |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | Spécifie une valeur booléenne indiquant si les informations de propriété des membres doivent être omises des infobulles du tableau croisé dynamique. |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | Indique si l'en-tête de colonne du tableau croisé dynamique doit recevoir le style appliqué. |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | Indique si le formatage en bandes est appliqué aux colonnes. |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | Indique si le formatage de la colonne est appliqué. |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | Indique si l'en-tête de ligne du tableau croisé dynamique doit recevoir le style appliqué. |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | Indique si le formatage en bandes des lignes est appliqué. |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | Indique s'il faut afficher les totaux généraux pour les lignes du tableau croisé dynamique. |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | Indique si la légende de l'en-tête de ligne est affichée dans le rapport du tableau croisé dynamique. Indique si les légendes des champs d'affichage et les listes déroulantes de filtre sont affichées. |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | Indique si la ligne des valeurs est affichée. |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | Indique si les éléments de champ de page masqués dans le rapport du tableau croisé dynamique sont inclus dans les sous-totaux des lignes et des colonnes, les totaux de bloc et les totaux généraux. |
| [setTag(String value)](#setTag-java.lang.String-) | Définit une chaîne définie par l'utilisateur associée à cette vue du PivotTable. |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | Afficher le détail d'un élément dans la région de données dans une nouvelle table. |
| [showInCompactForm()](#showInCompactForm--) | Mise en forme de la vue du tableau croisé dynamique sous forme compacte. |
| [showInOutlineForm()](#showInOutlineForm--) | Mise en forme du tableau croisé dynamique sous forme de plan. |
| [showInTabularForm()](#showInTabularForm--) | Mise en forme du tableau croisé dynamique sous forme tabulaire. |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | Afficher toutes les pages de filtre de rapport selon le PivotField, le PivotField doit être situé dans les PageFields. |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | Afficher toutes les pages de filtre de rapport selon l'index de position dans les PageFields. |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | Afficher toutes les pages de filtre de rapport selon le nom du PivotField, le PivotField doit être situé dans les PageFields. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


Ajoute un champ calculé au champ pivot et le fait glisser vers la zone de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom du champ calculé |
| formula | java.lang.String | La formule du champ calculé. |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


Ajoute un champ calculé au champ pivot.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom du champ calculé |
| formula | java.lang.String | La formule du champ calculé. |
| dragToDataArea | boolean | Vrai, faites glisser ce champ vers la zone de données immédiatement |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


Ajoute le champ à la zone spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). le type de zone des champs. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | le champ dans les champs de base. |

**Returns:**
int - la position du champ dans les champs spécifiques.
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Ajoute le champ à la zone spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Le type de zone des champs. |
| baseFieldIndex | int | L'index dans les champs de base. |

**Returns:**
int - La position du champ dans les champs spécifiques.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Ajoute le champ à la zone spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Le type de zone des champs. |
| fieldName | java.lang.String | Le nom dans les champs de base. |

**Returns:**
int - La position du champ dans les champs spécifiques. Si aucun champ ne porte ce nom, retourner -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Calcule les données du tableau croisé dynamique vers les cellules.

**Remarks**

Cette méthode ne calcule les données qu'avec les données mises en cache dans le [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). Ainsi, si vous souhaitez calculer avec la source de données la plus récente, veuillez utiliser la méthode [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) pour calculer. Si seul le paramètre du tableau croisé dynamique a été modifié, [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) suffit.

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public PivotTable[] calculateData(PivotTableCalculateOption option)
```


Calcule le tableau croisé dynamique avec des options.

**Remarks**

Si [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) est vrai, cette méthode rafraîchira le cache du tableau croisé dynamique depuis la source de données, puis calculera tous les tableaux croisés dynamiques basés sur le même cache. Sinon, le calcul ne se fera qu'avec les données mises en cache dans le cache du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | Les options pour calculer le tableau croisé dynamique |

**Returns:**
com.aspose.cells.PivotTable[] - Retourne tous les tableaux croisés dynamiques qui ont été calculés. Si [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) est vrai, tous les tableaux croisés dynamiques basés sur le même cache seront calculés ensemble.
### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


Calcule la plage du tableau croisé dynamique.

**Remarks**

Si cette méthode n'a pas été appelée, il se peut que la plage du tableau croisé dynamique ne soit pas correcte.

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


Modifie la source de données du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.lang.String[] |  |

### clearAll() {#clearAll--}
```
public void clearAll()
```


Supprime tous les champs des régions.

### clearData() {#clearData--}
```
public void clearData()
```


Efface les données et le formatage de la vue du tableau croisé dynamique.

**Remarks**

Si cette méthode n'est pas appelée avant d'ajouter ou de supprimer un PivotField, il se peut que les données du PivotTable ne soient pas corrigées

### clearFilters() {#clearFilters--}
```
public void clearFilters()
```


Efface tous les filtres de ce tableau croisé dynamique.

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


Copie le style nommé d'un autre tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Tableau croisé dynamique source. |

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
### exportViewToJson(PivotViewToJsonOptions options) {#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-}
```
public String exportViewToJson(PivotViewToJsonOptions options)
```


Exporte la vue du tableau croisé dynamique au format JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [PivotViewToJsonOptions](../../com.aspose.cells/pivotviewtojsonoptions) |  |

**Returns:**
java.lang.String -
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


Obtient les champs spécifiques par type de champ.

**Remarks**

REMARQUE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.GetFields(PivotFieldType). Cette méthode sera supprimée 12 mois plus tard à compter de mai 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). le type de champ. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


Formate la zone sélectionnée du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage des cellules. |
| style | [Style](../../com.aspose.cells/style) | Le style |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


Formate la zone sélectionnée du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | La zone de vue pivot sélectionnée. |
| style | [Style](../../com.aspose.cells/style) | Le paramètre formaté. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


Formate la cellule dans la zone du tableau croisé dynamique

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Index de ligne de la cellule |
| colonne | int | Indice de colonne de la cellule |
| style | [Style](../../com.aspose.cells/style) | Style utilisé pour formater la cellule |

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


Formate toutes les cellules dans la zone du tableau croisé dynamique

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Style utilisé pour formater |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


Formate les données de ligne dans la zone du tableau croisé dynamique

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Index de ligne de l'objet Row |
| style | [Style](../../com.aspose.cells/style) | Style utilisé pour formater |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués.

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


Obtient la description du texte alternatif.

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


Obtient le titre du texte alternatif.

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


Obtient le type de formatage automatique du tableau croisé dynamique.

Voir [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


Indique s'il faut ajuster automatiquement la largeur des colonnes lors de la mise à jour

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


Renvoie tous les champs de base du tableau croisé dynamique.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


Obtient la zone contenant le bouton de champ.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Le type de région. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


Obtient l'objet [Cell](../../com.aspose.cells/cell) par le nom d'affichage du PivotField.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| displayName | java.lang.String | le DisplayName du PivotField |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


Obtient les tableaux croisés dynamiques enfants qui utilisent les données de ce tableau croisé dynamique comme source de données.

**Remarks**

REMARQUE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.GetDependentPivotTables(). Cette méthode sera supprimée 12 mois plus tard à compter d'avril 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
com.aspose.cells.PivotTable[] - l'objet tableau PivotTable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnFields() {#getColumnFields--}
```
public PivotFieldCollection getColumnFields()
```


Renvoie un objet PivotFields qui est actuellement affiché comme champs de colonne.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


Indique si le rapport du tableau croisé dynamique affiche les totaux généraux pour les colonnes.

**Remarks**

REMARQUE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.ShowColumnGrandTotals. Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


Obtient la légende personnalisée de l'en-tête de colonne du tableau croisé dynamique.

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


Renvoie un objet CellArea qui représente la plage contenant la zone de colonne dans le rapport PivotTable. Lecture seule.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


Obtient les formats conditionnels du tableau croisé dynamique.

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


Indique s'il faut prendre en compte la liste personnalisée intégrée lors du tri des données

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


Renvoie un objet [CellArea](../../com.aspose.cells/cellarea) qui représente la plage contenant la zone de données dans la liste entre la ligne d'en-tête et la ligne d'insertion. Lecture seule.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


Obtient un objet [PivotField](../../com.aspose.cells/pivotfield) qui représente tous les champs de données d'un PivotTable. Lecture seule. Il n'est créé que lorsqu'il y a deux champs de données ou plus dans la région Data. Par défaut, il se trouve dans la région des lignes. Vous pouvez le faire glisser vers la région ligne/colonne avec la méthode PivotTable.AddFieldToArea().

**Remarks**

REMARQUE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.ValuesField. Cette méthode sera supprimée 12 mois plus tard à compter d'octobre 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


Obtient le nom de l’en-tête du champ de la zone de valeurs dans le tableau croisé dynamique.

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


Obtient une [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) qui représente tous les champs de données d’un tableau croisé dynamique.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


Obtient la source de données du tableau croisé dynamique.

**Returns:**
java.lang.String[]
### getDependentPivotTables() {#getDependentPivotTables--}
```
public PivotTable[] getDependentPivotTables()
```


Obtient tous les [PivotTable](../../com.aspose.cells/pivottable)s qui utilisent ce tableau croisé dynamique comme source de données.

**Remarks**

Comme les tableaux croisés dynamiques peuvent dépendre des données les uns des autres, ils doivent être actualisés dans le bon ordre afin d'assurer la cohérence des données.

**Returns:**
com.aspose.cells.PivotTable[] -
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


Indique si le rapport du tableau croisé dynamique affiche une chaîne personnalisée dans les cellules contenant des erreurs.

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


Indique si les éléments des zones de lignes et de colonnes sont visibles lorsque la zone de données du tableau croisé dynamique est vide. La valeur par défaut est true.

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


Indique si le rapport du tableau croisé dynamique affiche une chaîne personnalisée si la valeur est nulle.

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


Spécifie une valeur booléenne qui indique si l'utilisateur est autorisé à modifier les cellules de la zone de données du tableau croisé dynamique. La valeur par défaut est false.

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


Indique si le drilldown est activé.

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


Indique si la boîte de dialogue Champ du tableau croisé dynamique est disponible lorsque l’utilisateur double-clique sur le champ du tableau croisé dynamique.

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


Indique si la liste des champs du tableau croisé dynamique est disponible dans la vue d’Excel.

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


Indique si l’assistant Tableau croisé dynamique est disponible.

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide.

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


Obtient la source de données de connexion externe.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.GetSourceDataConnections(). Cette méthode sera supprimée 12 mois plus tard à compter d'octobre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


Indique si les champs du tableau croisé dynamique sont triés dans un ordre non par défaut dans la liste des champs.

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


Obtient la liste de champs pivot spécifique par région.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). le type de région. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


Obtient la zone de la région de filtre.

**Remarks**

Valide uniquement si des champs de filtre du tableau croisé dynamique existent. Une zone vide sera renvoyée si ce tableau croisé dynamique ne contient pas de champs de filtre.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


Renvoie l'étiquette affichée dans l'en-tête de colonne ou de ligne du total général. La valeur par défaut est la chaîne "Grand Total".

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


Obtient la liste des index de lignes du tableau croisé dynamique des sauts de page horizontaux.

**Remarks**

NOTE: Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.GetHorizontalPageBreaks(). Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.util.ArrayList -
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


Obtient les sauts de page horizontaux de ce tableau croisé dynamique.

**Returns:**
int[] -
### getIndent() {#getIndent--}
```
public int getIndent()
```


Spécifie l’incrément d’indentation pour l’axe compact et peut être utilisé pour définir la mise en page du rapport en forme compacte.

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


Indique si les noms de PivotItem doivent être répétés en haut de chaque page imprimée.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.RepeatItemsOnEachPrintedPage. Cette méthode sera supprimée 12 mois plus tard à compter d'octobre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


Indique si le rapport du tableau croisé dynamique est recalculé uniquement à la demande de l’utilisateur.

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


Obtient s’il faut fusionner les étiquettes de champs ligne/colonne qui s’étendent sur plusieurs cellules.

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués.

Voir [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotCache.MissingItemsLimit. Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtient le nom du tableau croisé dynamique

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


Obtient les noms des connexions de données source externes.

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


Obtient la chaîne affichée dans les cellules contenant des valeurs nulles lorsque la propriété DisplayNullString est vraie. La valeur par défaut est une chaîne vide.

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


Obtient l'ordre dans lequel les champs de page sont ajoutés à la disposition du rapport de tableau croisé dynamique.

Voir [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport de tableau croisé dynamique.

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


Renvoie une [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) qui sont actuellement affichées en tant que champs de page.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotCache() {#getPivotCache--}
```
public PivotCache getPivotCache()
```


Obtient la source de données.

**Returns:**
[PivotCache](../../com.aspose.cells/pivotcache)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


Renvoie tous les filtres du tableau croisé dynamique.

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


Obtient les conditions de format du tableau croisé dynamique.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.ConditionalFormats. Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


Obtient tous les formats de cellule appliqués à ce tableau croisé dynamique.

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


Obtient les paramètres de [TableStyle](../../com.aspose.cells/tablestyle) de ce tableau croisé dynamique.

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


Obtient le nom du style du tableau croisé dynamique.

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


Obtient le style intégré du tableau croisé dynamique.

Voir [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Returns:**
int
### getPivotTablesWithSamePivotCache() {#getPivotTablesWithSamePivotCache--}
```
public PivotTable[] getPivotTablesWithSamePivotCache()
```


Obtient tous les tableaux croisés dynamiques partageant le même cache de tableau croisé dynamique.

**Returns:**
com.aspose.cells.PivotTable[] -
### getPreserveCellFormattingOnUpdate() {#getPreserveCellFormattingOnUpdate--}
```
public boolean getPreserveCellFormattingOnUpdate()
```


Indique s'il faut préserver le format des cellules ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) lorsque le tableau croisé dynamique est actualisé ou recalculé.

**Returns:**
boolean
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Indique si le format des cellules ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) est préservé lorsque le tableau croisé dynamique est actualisé ou recalculé.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.PreserveCellFormattingOnUpdate. Cette méthode sera supprimée 12 mois plus tard à compter de juillet 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


Spécifie une valeur booléenne qui indique si les indicateurs de forage doivent être imprimés. Imprimez les boutons d'expansion/réduction lorsqu'ils sont affichés sur le tableau croisé dynamique.

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


Indique si les titres d'impression de la feuille de calcul sont définis en fonction du rapport du tableau croisé dynamique. La valeur par défaut est false.

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


Indique si l'option Refresh Data est activée lors de l'ouverture du fichier.

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


Obtient la date et l'heure de la dernière actualisation du tableau croisé dynamique.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


Obtient le nom du dernier utilisateur qui a actualisé ce tableau croisé dynamique.

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


Indique si les légendes des éléments de tableau croisé dynamique dans la zone de lignes sont répétées sur chaque page imprimée pour les champs de tableau croisé dynamique sous forme tabulaire.

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


Renvoie une [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) qui sont actuellement affichées en tant que champs de ligne.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


Indique s'il faut afficher les totaux généraux pour les lignes de ce tableau croisé dynamique.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.ShowRowGrandTotals. Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


Obtient la légende personnalisée de l'en-tête de ligne dans ce tableau croisé dynamique.

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


Renvoie un objet CellArea qui représente la plage contenant la zone de lignes dans le rapport du tableau croisé dynamique. Lecture seule.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Indique si les données du rapport de tableau croisé dynamique sont enregistrées avec le classeur.

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


Indique s'il faut afficher les totaux généraux pour les colonnes de ce tableau croisé dynamique.

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


Indique si les infobulles doivent être affichées pour les cellules de données du tableau croisé dynamique.

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


Obtient si l'affichage des boutons d'expansion/réduction est activé.

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


Indique s'il faut inclure les colonnes vides dans le tableau.

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


Indique s'il faut inclure les lignes vides dans le tableau.

**Returns:**
boolean
### getShowHeaders() {#getShowHeaders--}
```
public boolean getShowHeaders()
```


Indique s'il faut afficher les légendes des champs de données et les légendes des champs de tableau croisé dynamique sur l'axe des lignes et l'axe des colonnes dans la vue du tableau croisé dynamique.

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


Spécifie une valeur booléenne indiquant si les informations de propriété des membres doivent être omises des infobulles du tableau croisé dynamique.

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


Indique si l'en-tête de colonne du tableau croisé dynamique doit recevoir le style appliqué.

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


Indique si le formatage en bandes est appliqué aux colonnes.

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


Indique si le formatage de la colonne est appliqué.

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


Indique si l'en-tête de ligne du tableau croisé dynamique doit recevoir le style appliqué.

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


Indique si le formatage en bandes des lignes est appliqué.

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


Indique s'il faut afficher les totaux généraux pour les lignes du tableau croisé dynamique.

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


Indique si la légende de l'en-tête de ligne est affichée dans le rapport du tableau croisé dynamique. Indique si les légendes des champs d'affichage et les listes déroulantes de filtre sont affichées.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.ShowHeaders. Cette méthode sera supprimée 12 mois plus tard à compter d'avril 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


Indique si la ligne des valeurs est affichée.

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


Obtient la source de données de ce tableau croisé dynamique.

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


Obtient la source de données de ce tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isOriginal | boolean | Indique s'il faut renvoyer la source de données originale ou d'affichage. |

**Returns:**
java.lang.String[] -
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


Obtient les sources de données de connexion externes.

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


Obtient le type de source de données du tableau croisé dynamique.

Voir [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


Indique si les éléments de champ de page masqués dans le rapport du tableau croisé dynamique sont inclus dans les sous-totaux de lignes et de colonnes, les totaux de blocs et les totaux généraux. La valeur par défaut est False.

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport PivotTable, mais n'inclut pas les champs de page. Lecture seule.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport PivotTable, incluant les champs de page. Lecture seule.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


Obtient une chaîne définie par l'utilisateur associée à cette vue du tableau croisé dynamique.

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


Représente la zone vide en haut à droite du tableau croisé dynamique (en haut à gauche pour les feuilles RTL).

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


Obtient un objet [PivotField](../../com.aspose.cells/pivotfield) qui représente tous les champs de données d'un PivotTable. Lecture seule. Il n'est créé que lorsqu'il y a deux champs de données ou plus dans la région Data. Par défaut, il se trouve dans la région des lignes. Vous pouvez le faire glisser vers la région ligne/colonne avec la méthode PivotTable.AddFieldToArea().

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


Indique s'il faut ajouter des lignes vides. Cette propriété ne s'applique qu'aux types de formatage automatique de PivotTable qui nécessitent l'ajout de lignes vides.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.InsertBlankRow. Cette méthode sera supprimée 12 mois après, depuis avril 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFormat() {#isAutoFormat--}
```
public boolean isAutoFormat()
```


Indique si le rapport PivotTable est formaté automatiquement. Case à cocher "autoformat table" qui se trouve dans l'option pivottable pour Excel 2003.

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


Spécifie si le PivotTable est compatible avec Excel2003 lors du rafraîchissement du PivotTable ; si vrai, une chaîne doit contenir au maximum 255 caractères, sinon elle sera tronquée. Si faux, aucune restriction de ce type ne s'applique. La valeur par défaut est vraie.

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


Indique si le rapport PivotTable affiche la mise en page classique du pivottable. (permet le glisser‑déposer des champs dans la grille)

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotTable.AllowMultipleFiltersPerField. Cette méthode sera supprimée 12 mois après, depuis décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Indique si ce PivotTable est sélectionné.

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


Déplace le PivotTable vers un autre emplacement dans la feuille de calcul.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la méthode PivotTable.MoveTo(). Cette méthode sera supprimée 12 mois après, depuis décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | indice de ligne. |
| colonne | int | indice de colonne. |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


Déplace le PivotTable vers un autre emplacement dans la feuille de calcul.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la méthode PivotTable.MoveTo(). Cette méthode sera supprimée 12 mois après, depuis décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destCellName | java.lang.String | le nom de la cellule de destination. |

### moveItem(int region, String[] nodes, boolean absolute, int offset) {#moveItem-int-java.lang.String---boolean-int-}
```
public void moveItem(int region, String[] nodes, boolean absolute, int offset)
```


Déplace un élément vers le haut ou vers le bas.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| region | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). La région. Uniquement pour la ligne ou la colonne. |
| nœuds | java.lang.String[] | L'élément. |
| absolu | boolean | Indique si le décalage est une position absolue. |
| décalage | int | Si absolu est vrai : 0 déplace au début, -1 déplace à la fin, les autres indiquent une position absolue ; sinon le décalage est une position relative. |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


Déplace le PivotTable vers un autre emplacement dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | indice de ligne. |
| colonne | int | indice de colonne. |

### moveTo(int sheetIndex, int row, int column) {#moveTo-int-int-int-}
```
public void moveTo(int sheetIndex, int row, int column)
```


Déplace le PivotTable vers un autre emplacement dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | l'indice de la feuille de calcul cible |
| ligne | int | indice de ligne. |
| colonne | int | indice de colonne. |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


Déplace le PivotTable vers un autre emplacement dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destCellName | java.lang.String | le nom de la cellule de destination. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int refresh()
```


Actualise [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) depuis la source de données et calcule les données et le style pour la vue du pivot.

**Remarks**

Tous les tableaux croisés dynamiques qui dépendent du même PivotCache seront recalculés.

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Actualise [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) depuis la source de données et calcule les données et le style pour la vue du pivot.

**Remarks**

Tous les tableaux croisés dynamiques qui dépendent du même PivotCache seront recalculés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refreshData() {#refreshData--}
```
public int refreshData()
```


Actualise les données depuis sa source de données vers le cache du pivot.

**Remarks**

Nous collecterons les données de la source de données vers un cache de pivot, puis calculerons les données du cache dans les cellules. Il est préférable d'appeler simplement [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) pour actualiser et calculer tous les tableaux croisés dynamiques du fichier, au lieu de les actualiser un par un. NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser la méthode [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) et supprimer la méthode [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) qui suit, car ce tableau croisé dynamique sera calculé lors de l'actualisation de [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). Cette méthode sera supprimée 12 mois après, depuis juin 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


Actualise les données et les paramètres du PivotTable depuis sa source de données avec des options.

**Remarks**

Nous collecterons les données de la source de données vers un cache de pivot, puis calculerons les données du cache dans les cellules. Il est préférable d'appeler simplement [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) pour actualiser et calculer tous les tableaux croisés dynamiques du fichier, au lieu de les actualiser un par un. NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser la méthode [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) et supprimer la méthode [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) car ce tableau croisé dynamique sera calculé lors de l'actualisation de [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) Cette méthode sera supprimée 12 mois après, depuis juin 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Les options pour actualiser la source de données du tableau croisé dynamique. |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


Supprimer le champ d'une zone de champ spécifique

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). le type de zone des champs. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | le champ dans les champs de base. |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


Supprime un champ d'une région de pivot spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Le type de zone des champs. |
| baseFieldIndex | int | L'index du champ dans les champs de base. |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


Supprime un champ d'une zone de champ spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Le type de zone des champs. |
| fieldName | java.lang.String | Le nom dans les champs de base. |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


Sélectionner une zone de la vue du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La zone de cellule. |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


Obtient la description du texte alternatif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


Définit le titre du texte alternatif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


Indique si le rapport PivotTable est formaté automatiquement. Case à cocher "autoformat table" qui se trouve dans l'option pivottable pour Excel 2003.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


Définit le type de format automatique du PivotTable.

Voir [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


Indique s'il faut ajuster automatiquement la largeur des colonnes lors de la mise à jour

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


Indique si le rapport du tableau croisé dynamique affiche les totaux généraux pour les colonnes.

**Remarks**

REMARQUE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.ShowColumnGrandTotals. Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


Définit la légende personnalisée de l'en-tête de colonne du PivotTable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


Indique s'il faut prendre en compte la liste personnalisée intégrée lors du tri des données

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


Définit le nom de l'en-tête du champ de la zone de valeurs dans le PivotTable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


Définit la source de données du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


Indique si le rapport du tableau croisé dynamique affiche une chaîne personnalisée dans les cellules contenant des erreurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


Indique si les éléments des zones de lignes et de colonnes sont visibles lorsque la zone de données du tableau croisé dynamique est vide. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


Indique si le rapport du tableau croisé dynamique affiche une chaîne personnalisée si la valeur est nulle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


Spécifie une valeur booléenne qui indique si l'utilisateur est autorisé à modifier les cellules de la zone de données du tableau croisé dynamique. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


Indique si le drilldown est activé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


Indique si la boîte de dialogue Champ du tableau croisé dynamique est disponible lorsque l’utilisateur double-clique sur le champ du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


Indique si la liste des champs du tableau croisé dynamique est disponible dans la vue d’Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


Indique si l’assistant Tableau croisé dynamique est disponible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


Spécifie si le PivotTable est compatible avec Excel2003 lors du rafraîchissement du PivotTable ; si vrai, une chaîne doit contenir au maximum 255 caractères, sinon elle sera tronquée. Si faux, aucune restriction de ce type ne s'applique. La valeur par défaut est vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


Indique si les champs du tableau croisé dynamique sont triés dans un ordre non par défaut dans la liste des champs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


Renvoie l'étiquette affichée dans l'en-tête de colonne ou de ligne du total général. La valeur par défaut est la chaîne "Grand Total".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


Indique si le rapport PivotTable affiche la mise en page classique du pivottable. (permet le glisser‑déposer des champs dans la grille)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


Indique s'il faut ajouter des lignes vides. Cette propriété ne s'applique qu'aux types de formatage automatique de PivotTable qui nécessitent l'ajout de lignes vides.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.InsertBlankRow. Cette méthode sera supprimée 12 mois après, depuis avril 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


Spécifie l’incrément d’indentation pour l’axe compact et peut être utilisé pour définir la mise en page du rapport en forme compacte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


Indique si les noms de PivotItem doivent être répétés en haut de chaque page imprimée.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.RepeatItemsOnEachPrintedPage. Cette méthode sera supprimée 12 mois plus tard à compter d'octobre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


Indique si le rapport du tableau croisé dynamique est recalculé uniquement à la demande de l’utilisateur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


Définit s'il faut fusionner les libellés de champs ligne/colonne qui s'étendent sur plusieurs cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués.

Voir [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotCache.MissingItemsLimit. Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


Spécifie une valeur booléenne indiquant si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotTable.AllowMultipleFiltersPerField. Cette méthode sera supprimée 12 mois après, depuis décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Obtient le nom du tableau croisé dynamique

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


Obtient la chaîne affichée dans les cellules contenant des valeurs nulles lorsque la propriété DisplayNullString est vraie. La valeur par défaut est une chaîne vide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


Définit l'ordre dans lequel les champs de page sont ajoutés à la mise en page du rapport PivotTable.

Voir [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport de tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


Obtient les paramètres de [TableStyle](../../com.aspose.cells/tablestyle) de ce tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


Définit le nom du style du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


Définit le style intégré du tableau croisé dynamique.

Voir [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPreserveCellFormattingOnUpdate(boolean value) {#setPreserveCellFormattingOnUpdate-boolean-}
```
public void setPreserveCellFormattingOnUpdate(boolean value)
```


Indique s'il faut préserver le format des cellules ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) lorsque le tableau croisé dynamique est actualisé ou recalculé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Indique si le format des cellules ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) est préservé lorsque le tableau croisé dynamique est actualisé ou recalculé.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.PreserveCellFormattingOnUpdate. Cette méthode sera supprimée 12 mois plus tard à compter de juillet 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


Spécifie une valeur booléenne qui indique si les indicateurs de forage doivent être imprimés. Imprimez les boutons d'expansion/réduction lorsqu'ils sont affichés sur le tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


Indique si les titres d'impression de la feuille de calcul sont définis en fonction du rapport du tableau croisé dynamique. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


Indique si l'option Refresh Data est activée lors de l'ouverture du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


Indique si les légendes des éléments de tableau croisé dynamique dans la zone de lignes sont répétées sur chaque page imprimée pour les champs de tableau croisé dynamique sous forme tabulaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


Indique s'il faut afficher les totaux généraux pour les lignes de ce tableau croisé dynamique.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.ShowRowGrandTotals. Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


Définit la légende personnalisée de l'en-tête de ligne dans ce PivotTable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Indique si les données du rapport de tableau croisé dynamique sont enregistrées avec le classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indique si ce PivotTable est sélectionné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


Indique s'il faut afficher les totaux généraux pour les colonnes de ce tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


Indique si les infobulles doivent être affichées pour les cellules de données du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


Définit s'il faut afficher les boutons d'extension/réduction.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


Indique s'il faut inclure les colonnes vides dans le tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


Indique s'il faut inclure les lignes vides dans le tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowHeaders(boolean value) {#setShowHeaders-boolean-}
```
public void setShowHeaders(boolean value)
```


Indique s'il faut afficher les légendes des champs de données et les légendes des champs de tableau croisé dynamique sur l'axe des lignes et l'axe des colonnes dans la vue du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


Spécifie une valeur booléenne indiquant si les informations de propriété des membres doivent être omises des infobulles du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


Indique si l'en-tête de colonne du tableau croisé dynamique doit recevoir le style appliqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


Indique si le formatage en bandes est appliqué aux colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


Indique si le formatage de la colonne est appliqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


Indique si l'en-tête de ligne du tableau croisé dynamique doit recevoir le style appliqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


Indique si le formatage en bandes des lignes est appliqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


Indique s'il faut afficher les totaux généraux pour les lignes du tableau croisé dynamique.

**Remarks**

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


Indique si la légende de l'en-tête de ligne est affichée dans le rapport du tableau croisé dynamique. Indique si les légendes des champs d'affichage et les listes déroulantes de filtre sont affichées.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.ShowHeaders. Cette méthode sera supprimée 12 mois plus tard à compter d'avril 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


Indique si la ligne des valeurs est affichée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


Indique si les éléments de champ de page masqués dans le rapport du tableau croisé dynamique sont inclus dans les sous-totaux de lignes et de colonnes, les totaux de blocs et les totaux généraux. La valeur par défaut est False.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


Définit une chaîne définie par l'utilisateur associée à cette vue du PivotTable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


Afficher le détail d'un élément dans la région de données dans une nouvelle table.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | Décalage vers la première ligne de données dans la région de données. |
| columnOffset | int | Décalage vers la première colonne de données dans la région de données. |
| newSheet | boolean | Afficher le détail dans une nouvelle feuille de calcul. |
| destRow | int | La ligne cible. |
| destColumn | int | La colonne cible. |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


Mise en forme de la vue du tableau croisé dynamique sous forme compacte.

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


Mise en forme du tableau croisé dynamique sous forme de plan.

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


Mise en forme du tableau croisé dynamique sous forme tabulaire.

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


Afficher toutes les pages de filtre de rapport selon le PivotField, le PivotField doit être situé dans les PageFields.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | L'objet PivotField |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


Afficher toutes les pages de filtre de rapport selon l'index de position dans les PageFields.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| posIndex | int | L'index de position dans les PageFields |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


Afficher toutes les pages de filtre de rapport selon le nom du PivotField, le PivotField doit être situé dans les PageFields.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | Le nom de PivotField |

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

