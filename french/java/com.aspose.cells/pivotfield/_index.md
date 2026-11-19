---
title: "PivotField"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un champ dans un rapport de tableau croisé dynamique."
type: docs
url: /fr/java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

Représente un champ dans un rapport de tableau croisé dynamique.

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
 
          pivot.calculateData(new PivotTableCalculateOption());
 
         //do your business
 
         book.save("out.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | Ajoutez un élément de formule calculée au champ pivot. |
| [clearFilter()](#clearFilter--) | Efface les paramètres de filtre sur ce champ pivot. |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtre par valeurs de date du champ pivot de ligne ou de colonne. |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | Filtre par légendes du champ pivot de ligne ou de colonne. |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | Filtre par valeurs du champ pivot de données. |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | Filtre par valeurs du champ pivot de données. |
| [getAllowDraggingToColumn()](#getAllowDraggingToColumn--) | Indique si le champ spécifié peut être glissé vers la région des colonnes. |
| [getAllowDraggingToData()](#getAllowDraggingToData--) | Indique si le champ spécifié peut être glissé vers la région des valeurs. |
| [getAllowDraggingToPage()](#getAllowDraggingToPage--) | Indique si le champ spécifié peut être glissé vers la région de la page. |
| [getAllowDraggingToRow()](#getAllowDraggingToRow--) | Indique si le champ spécifié peut être glissé vers la région des lignes. |
| [getAllowRemovingFromView()](#getAllowRemovingFromView--) | Indique si ce champ pivot peut être supprimé de la vue du tableau croisé dynamique. |
| [getAutoShowCount()](#getAutoShowCount--) | Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ de tableau croisé dynamique spécifié. |
| [getAutoShowField()](#getAutoShowField--) | Représente l'index du champ d'affichage automatique. -1 signifie le champ PivotField lui‑même. |
| [getAutoSortField()](#getAutoSortField--) | Représente l'index du champ qui est trié automatiquement |
| [getBaseIndex()](#getBaseIndex--) | Représente l'index dans les champs pivot source. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | Obtenez la chaîne de formule du champ calculé spécifié. |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | Obtient l'élément de page actuellement affiché pour ce champ pivot (champ de page uniquement). |
| [getCurrentPageItemText()](#getCurrentPageItemText--) | Obtient le texte d'affichage de l'élément de page actuel pour ce champ de tableau croisé dynamique (champ de page uniquement). |
| [getDisplayName()](#getDisplayName--) | Représente le nom d'affichage du champ de tableau croisé dynamique dans la vue du tableau croisé dynamique. |
| [getDragToColumn()](#getDragToColumn--) | Indique si le champ spécifié peut être glissé vers la région des colonnes. |
| [getDragToData()](#getDragToData--) | Indique si le champ spécifié peut être glissé vers la région des valeurs. |
| [getDragToHide()](#getDragToHide--) | Indique si ce champ pivot peut être supprimé de la vue du tableau croisé dynamique. |
| [getDragToPage()](#getDragToPage--) | Indique si le champ spécifié peut être glissé vers la région de la page. |
| [getDragToRow()](#getDragToRow--) | Indique si le champ spécifié peut être glissé vers la région des lignes. |
| [getFilters()](#getFilters--) | Obtient tous les filtres de tableau croisé dynamique appliqués à ce champ de tableau croisé dynamique. |
| [getFormula()](#getFormula--) | Obtient la formule du champ calculé. |
| [getFunction()](#getFunction--) | Représente la fonction utilisée pour résumer ce champ de données du tableau croisé dynamique. |
| [getGroupSettings()](#getGroupSettings--) | Obtient les paramètres de groupe du champ de tableau croisé dynamique. |
| [getInsertBlankRow()](#getInsertBlankRow--) | Indique s'il faut insérer une ligne vide après chaque élément. |
| [getItemCount()](#getItemCount--) | Obtient le nombre d'éléments de base dans ce champ de tableau croisé dynamique. |
| [getItems()](#getItems--) | Obtenez toutes les étiquettes des éléments de tableau croisé dynamique dans ce champ. |
| [getMaxValue()](#getMaxValue--) | Obtient la valeur maximale de ce champ. |
| [getMinValue()](#getMinValue--) | Obtient la valeur maximale de ce champ. |
| [getName()](#getName--) | Représente le nom de PivotField. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | Indique si une opération de tri qui sera appliquée à ce champ de tableau croisé dynamique est une opération de tri automatique ou un tri de données simple. |
| [getNumber()](#getNumber--) | Représente le format d'affichage intégré des nombres et des dates. |
| [getNumberFormat()](#getNumberFormat--) | Représente le format d'affichage personnalisé des nombres et des dates. |
| [getOriginalItems()](#getOriginalItems--) | Obtenez les éléments de base originaux; |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | Obtient le filtre de tableau croisé dynamique du champ de tableau croisé dynamique par type |
| [getPivotFilters()](#getPivotFilters--) | Obtient les filtres de tableau croisé dynamique du champ de tableau croisé dynamique |
| [getPivotItems()](#getPivotItems--) | Obtient les éléments de tableau croisé dynamique du champ de tableau croisé dynamique |
| [getPosition()](#getPosition--) | Représente l'index de [PivotField](../../com.aspose.cells/pivotfield) dans la région. |
| [getRegionType()](#getRegionType--) | Spécifie la région du tableau croisé dynamique où ce champ est affiché. |
| [getShowAllItems()](#getShowAllItems--) | Indique s'il faut afficher tous les éléments dans la vue du tableau croisé dynamique, même s'ils ne contiennent pas de données de synthèse. |
| [getShowCompact()](#getShowCompact--) | Indique s'il faut afficher les étiquettes du champ suivant dans la même colonne dans la vue du tableau croisé dynamique. |
| [getShowInCompactForm()](#getShowInCompactForm--) | Obtient une valeur indiquant si ce champ de ligne utilise la disposition en forme compacte. |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Obtient une valeur indiquant si ce champ de ligne utilise la disposition en plan. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | Indique s'il faut afficher les sous-totaux en haut ou en bas des éléments. |
| [getShowValuesSetting()](#getShowValuesSetting--) | Obtient les paramètres d'affichage des valeurs comme lorsque le calcul ShowDataAs est utilisé. |
| [getSortSetting()](#getSortSetting--) | Obtient tous les paramètres du tri automatique |
| [getSubtotals()](#getSubtotals--) | Obtient les sous‑totaux du champ. |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Indique s'il faut afficher le sous‑total spécifié pour ce champ de tableau croisé dynamique. |
| [getTop10AutoShowSettings()](#getTop10AutoShowSettings--) | Obtient les paramètres AutoShow du Top 10 pour un champ de tableau croisé dynamique. |
| [group()](#group--) | Regroupe automatiquement le champ. |
| [group(PivotFieldGroupOptions options)](#group-com.aspose.cells.PivotFieldGroupOptions-) | Regroupe le champ de tableau croisé dynamique avec des options. |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | Regroupe le fichier par les types de groupe de dates. |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | Regroupe le fichier par numéro. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | Regroupe le champ de manière personnalisée. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | Regroupe le fichier par les types de groupe de dates. |
| [groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-) | Regroupe le champ de manière personnalisée. |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | Regroupe automatiquement le champ avec un intervalle |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | Regroupe le fichier par numéro. |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | Regroupe automatiquement le champ avec interne |
| [hashCode()](#hashCode--) |  |
| [hideAllDetails()](#hideAllDetails--) | Masque tous les détails de chaque élément de tableau croisé dynamique. |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | Définit si le détail de tous les PivotItems d'un champ de tableau croisé dynamique est masqué. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Définit si l'élément PivotItem spécifique d'un champ de données est masqué. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | Définit si l'élément PivotItem spécifique d'un champ de données est masqué. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | Définit si le détail de l'élément PivotItem spécifique d'un champ de tableau croisé dynamique est masqué. |
| [initPivotItems()](#initPivotItems--) | Initialise les éléments de tableau croisé dynamique du champ. |
| [isAscendShow()](#isAscendShow--) | Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement en ordre croissant. |
| [isAscendSort()](#isAscendSort--) | Indique si les éléments de ce champ de tableau croisé dynamique sont automatiquement triés par ordre croissant. |
| [isAutoShow()](#isAutoShow--) | Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement. |
| [isAutoSort()](#isAutoSort--) | Indique si les éléments de ce champ de tableau croisé dynamique sont triés automatiquement. |
| [isAutoSubtotals()](#isAutoSubtotals--) | Indique si le champ spécifié affiche des sous‑totaux automatiques. |
| [isCalculatedField()](#isCalculatedField--) | Indique si ce champ de tableau croisé dynamique est un champ calculé. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | Indique si l'élément PivotItem spécifique est masqué. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | Indique s'il faut masquer le détail de l'élément PivotItem spécifique.. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | Indique s'il faut inclure de nouveaux éléments au champ dans le filtre manuel. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | Indique s'il faut insérer des sauts de page après chaque élément. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | Indique si plusieurs éléments peuvent être sélectionnés dans le champ de page. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | Indique s'il faut répéter les libellés du champ dans la région ligne ou colonne. |
| [isValueFields()](#isValueFields--) | Indique si ce champ représente des champs de valeurs. |
| [isValuesField()](#isValuesField--) | Indique si ce champ représente un champ de valeurs. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDraggingToColumn(boolean value)](#setAllowDraggingToColumn-boolean-) | Indique si le champ spécifié peut être glissé vers la région des colonnes. |
| [setAllowDraggingToData(boolean value)](#setAllowDraggingToData-boolean-) | Indique si le champ spécifié peut être glissé vers la région des valeurs. |
| [setAllowDraggingToPage(boolean value)](#setAllowDraggingToPage-boolean-) | Indique si le champ spécifié peut être glissé vers la région de la page. |
| [setAllowDraggingToRow(boolean value)](#setAllowDraggingToRow-boolean-) | Indique si le champ spécifié peut être glissé vers la région des lignes. |
| [setAllowRemovingFromView(boolean value)](#setAllowRemovingFromView-boolean-) | Indique si ce champ pivot peut être supprimé de la vue du tableau croisé dynamique. |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement en ordre croissant. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Indique si les éléments de ce champ de tableau croisé dynamique sont automatiquement triés par ordre croissant. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ de tableau croisé dynamique spécifié. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Représente l'index du champ d'affichage automatique. -1 signifie le champ PivotField lui‑même. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Indique si les éléments de ce champ de tableau croisé dynamique sont triés automatiquement. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Représente l'index du champ qui est trié automatiquement |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Indique si le champ spécifié affiche des sous‑totaux automatiques. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Représente l'index dans les champs pivot source. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Définit l'élément de page actuellement affiché pour ce champ de tableau croisé dynamique (champ de page uniquement). |
| [setCurrentPageItemText(String value)](#setCurrentPageItemText-java.lang.String-) | Obtient le texte d'affichage de l'élément de page actuel pour ce champ de tableau croisé dynamique (champ de page uniquement). |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Représente le nom d'affichage du champ de tableau croisé dynamique dans la vue du tableau croisé dynamique. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Indique si le champ spécifié peut être glissé vers la région des colonnes. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Indique si le champ spécifié peut être glissé vers la région des valeurs. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Indique si ce champ pivot peut être supprimé de la vue du tableau croisé dynamique. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Indique si le champ spécifié peut être glissé vers la région de la page. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Indique si le champ spécifié peut être glissé vers la région des lignes. |
| [setFunction(int value)](#setFunction-int-) | Représente la fonction utilisée pour résumer ce champ de données du tableau croisé dynamique. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | Indique s'il faut inclure de nouveaux éléments au champ dans le filtre manuel. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Indique s'il faut insérer une ligne vide après chaque élément. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | Indique s'il faut insérer des sauts de page après chaque élément. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | Indique si plusieurs éléments peuvent être sélectionnés dans le champ de page. |
| [setName(String value)](#setName-java.lang.String-) | Représente le nom de PivotField. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Indique si une opération de tri qui sera appliquée à ce champ de tableau croisé dynamique est une opération de tri automatique ou un tri de données simple. |
| [setNumber(int value)](#setNumber-int-) | Représente le format d'affichage intégré des nombres et des dates. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Représente le format d'affichage personnalisé des nombres et des dates. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | Indique s'il faut répéter les libellés du champ dans la région ligne ou colonne. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Indique s'il faut afficher tous les éléments dans la vue du tableau croisé dynamique, même s'ils ne contiennent pas de données de synthèse. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Indique s'il faut afficher les étiquettes du champ suivant dans la même colonne dans la vue du tableau croisé dynamique. |
| [setShowInCompactForm(boolean value)](#setShowInCompactForm-boolean-) | Définit une valeur indiquant si ce champ de ligne utilise la disposition en forme compacte. |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Définit une valeur indiquant si ce champ de ligne utilise la disposition en plan. |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | Indique s'il faut afficher les sous-totaux en haut ou en bas des éléments. |
| [setSubtotals(int value)](#setSubtotals-int-) | Définit les sous-totaux du champ. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Définit comment sous-totaliser le champ spécifié. |
| [showAllDetails()](#showAllDetails--) | Afficher tous les détails de chaque élément de tableau croisé dynamique. |
| [showValuesAs(int showValuesAsType, int baseField, int baseItem)](#showValuesAs-int-int-int-) | Définit le calcul « Afficher les valeurs sous forme de » pour ce champ de tableau croisé dynamique. |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | Affiche les valeurs du champ de données dans un format d'affichage différent lorsque le calcul ShowDataAs est utilisé. |
| [showValuesAs(int showValuesAsType, String baseField, String baseItem)](#showValuesAs-int-java.lang.String-java.lang.String-) | Configure le calcul « Afficher les valeurs sous forme de » pour ce champ de données. |
| [sortBy(int sortType)](#sortBy-int-) | Trie ce champ de tableau croisé dynamique. |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | Trie ce champ de tableau croisé dynamique. |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | Trie ce champ de tableau croisé dynamique. |
| [sortBy(int sortType, int fieldSortedBy, String cellName)](#sortBy-int-int-java.lang.String-) | Trie ce champ de tableau croisé dynamique. |
| [toString()](#toString--) |  |
| [top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)](#top10AutoShow-boolean-boolean-int-int-) | Configure les paramètres Top10 AutoShow pour ce champ de tableau croisé dynamique. |
| [ungroup()](#ungroup--) | Dégrouper le champ de tableau croisé dynamique. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Ajoutez un élément de formule calculée au champ pivot.

**Remarks**

Ne prend en charge que l'ajout d'un élément calculé au champ Ligne/Colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de l'élément. |
| formula | java.lang.String | La formule de l'élément de tableau croisé dynamique. |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Efface les paramètres de filtre sur ce champ pivot.

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
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


Filtre par valeurs de date du champ pivot de ligne ou de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Le type de filtrage des données. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | L'étiquette de date de la condition de filtrage |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | L'étiquette de date supérieure de la condition de filtrage entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


Filtre par légendes du champ pivot de ligne ou de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Le type de filtrage des données. |
| label1 | java.lang.String | L'étiquette de la condition de filtrage |
| label2 | java.lang.String | L'étiquette supérieure de la condition de filtre entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


Filtre par valeurs du champ pivot de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valueFieldIndex | int | L'index du champ de valeur dans la région de valeur. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Le type de filtrage des données. |
| value1 | double | La valeur de la condition de filtre |
| value2 | double | La valeur supérieure de la condition de filtre entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtre par valeurs du champ pivot de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valueFieldIndex | int | L'index du champ de données dans la région de données. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Le type de filtrage des données. Peut uniquement être Count,Sum et Percent. |
| isTop | boolean | Indique si le filtre provient du haut ou du bas |
| itemCount | int | Le nombre d'éléments |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAllowDraggingToColumn() {#getAllowDraggingToColumn--}
```
public boolean getAllowDraggingToColumn()
```


Indique si le champ spécifié peut être glissé vers la région colonne. La valeur par défaut est vraie.

**Returns:**
boolean
### getAllowDraggingToData() {#getAllowDraggingToData--}
```
public boolean getAllowDraggingToData()
```


Indique si le champ spécifié peut être glissé vers la région valeurs. La valeur par défaut est vraie.

**Returns:**
boolean
### getAllowDraggingToPage() {#getAllowDraggingToPage--}
```
public boolean getAllowDraggingToPage()
```


Indique si le champ spécifié peut être glissé vers la région page. La valeur par défaut est vraie.

**Returns:**
boolean
### getAllowDraggingToRow() {#getAllowDraggingToRow--}
```
public boolean getAllowDraggingToRow()
```


Indique si le champ spécifié peut être glissé vers la région ligne. La valeur par défaut est vraie.

**Returns:**
boolean
### getAllowRemovingFromView() {#getAllowRemovingFromView--}
```
public boolean getAllowRemovingFromView()
```


Indique si ce champ de tableau croisé dynamique peut être supprimé de la vue du tableau croisé dynamique. La valeur par défaut est vraie.

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ de tableau croisé dynamique spécifié.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.Top10AutoShowSettings.AutoShowCount ou la méthode PivotField.Top10AutoShow(). Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


Représente l'index du champ d'affichage automatique. -1 signifie le PivotField lui‑même. Il doit s'agir de l'index des champs de données.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.Top10AutoShowSettings.RankBy ou la méthode PivotField.Top10AutoShow(). Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


Représente l'index du champ qui est trié automatiquement. -1 signifie le PivotField lui‑même, les autres valeurs indiquent la position des champs de données.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.SortSetting.SortBy ou la méthode PivotField.SortBy(). Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


Représente l'index dans les champs pivot source.

**Remarks**

NOTE : Le mutateur de cette propriété est maintenant obsolète. Ce mutateur sera supprimé 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


Obtenez la chaîne de formule du champ calculé spécifié.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser la méthode PivotField.GetFormula(). Cette méthode sera supprimée 12 mois plus tard, à compter d'août 2024. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageItem() {#getCurrentPageItem--}
```
public short getCurrentPageItem()
```


Obtient l'élément de page actuellement affiché pour ce champ pivot (champ de page uniquement).

**Remarks**

Utilisez [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) comme valeur sentinelle pour indiquer "Select All". Il s'agit d'un marqueur prédéfini et ce n'est pas un index d'élément valide.

**Returns:**
short
### getCurrentPageItemText() {#getCurrentPageItemText--}
```
public String getCurrentPageItemText()
```


Obtient le texte d'affichage de l'élément de page actuel pour ce champ de tableau croisé dynamique (champ de page uniquement).

**Remarks**

Renvoie "(All)" lorsque [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--) est égal à [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX). Pour les autres valeurs, renvoie la représentation sous forme de chaîne de l'index de l'élément.

**Returns:**
java.lang.String
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Représente le nom d'affichage du champ de tableau croisé dynamique dans la vue du tableau croisé dynamique.

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


Indique si le champ spécifié peut être glissé vers la région colonne. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToColumn. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


Indique si le champ spécifié peut être glissé vers la région valeurs. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToData. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


Indique si ce champ de tableau croisé dynamique peut être supprimé de la vue du tableau croisé dynamique. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowRemovingFromView. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


Indique si le champ spécifié peut être glissé vers la région page. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToPage. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


Indique si le champ spécifié peut être glissé vers la région ligne. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToRow. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


Obtient tous les filtres de tableau croisé dynamique appliqués à ce champ de tableau croisé dynamique.

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtient la formule du champ calculé. Fonctionne uniquement pour le champ calculé.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


Représente la fonction utilisée pour résumer ce champ de données du tableau croisé dynamique.

Voir [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


Obtient les paramètres de groupe du champ de tableau croisé dynamique.

**Remarks**

Si ce champ n'est pas groupé, Null sera renvoyé.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


Indique s'il faut insérer une ligne vide après chaque élément. Seulement pour les champs de ligne.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


Obtient le nombre d'éléments de base dans ce champ de tableau croisé dynamique.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.PivotItems.Count. Cette méthode sera supprimée 12 mois plus tard, à compter d'août 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


Obtenez toutes les étiquettes des éléments de tableau croisé dynamique dans ce champ.

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


Obtient la valeur maximale de ce champ.

**Remarks**

Fonctionne uniquement pour les champs de ligne ou de colonne dont la valeur doit être une date/heure, un nombre ou vide.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


Obtient la valeur maximale de ce champ.

**Remarks**

Fonctionne uniquement pour les champs de ligne ou de colonne dont la valeur doit être une date/heure, un nombre ou vide.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


Représente le nom de PivotField.

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


Indique si une opération de tri qui sera appliquée à ce champ de tableau croisé dynamique est une opération de tri automatique ou un tri de données simple.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété !PivotField.SortSetting.IsSimpleSort. Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


Représente le format d'affichage intégré des nombres et des dates.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Représente le format d'affichage personnalisé des nombres et des dates.

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


Obtenez les éléments de base originaux;

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


Obtient le filtre de tableau croisé dynamique du champ de tableau croisé dynamique par type

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


Obtient les filtres de tableau croisé dynamique du champ de tableau croisé dynamique

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.GetFilters() method. Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2023. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


Obtient les éléments de tableau croisé dynamique du champ de tableau croisé dynamique

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Représente l'index de [PivotField](../../com.aspose.cells/pivotfield) dans la région.

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


Spécifie la région du tableau croisé dynamique où ce champ est affiché.

Voir [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Indique si tous les éléments doivent être affichés dans la vue du tableau croisé dynamique, même s'ils ne contiennent pas de données récapitulatives. La valeur par défaut est false.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


Indique si les étiquettes du champ suivant doivent être affichées dans la même colonne dans la vue du tableau croisé dynamique. Uniquement pour les champs de ligne.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.ShowInCompactForm property instead . Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
boolean
### getShowInCompactForm() {#getShowInCompactForm--}
```
public boolean getShowInCompactForm()
```


Obtient une valeur indiquant si ce champ de ligne utilise la disposition en forme compacte. S'applique uniquement aux champs de ligne.

**Remarks**

La forme compacte est un sous-mode de la disposition en plan. Ce paramètre ne prend effet que lorsque [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) est vrai.

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


Obtient une valeur indiquant si ce champ de ligne utilise la disposition en plan. S'applique uniquement aux champs de ligne.

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


Indique s'il faut afficher les sous-totaux en haut ou en bas des éléments.

**Remarks**

Ne fonctionne que pour les champs de pivot dans la région des lignes lorsque ShowInOutlineForm est vrai.

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


Obtient les paramètres d'affichage des valeurs comme lorsque le calcul ShowDataAs est utilisé.

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


Obtient tous les paramètres du tri automatique

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals() {#getSubtotals--}
```
public int getSubtotals()
```


Obtient les sous‑totaux du champ. Uniquement pour les champs de pivot de ligne ou de colonne.

Voir [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Example**

```
         //No subtotals
         rowField.setSubtotals(PivotFieldSubtotalType.NONE);
         //Automatic subtotals
         //rowField.Subtotals = PivotFieldSubtotalType.Automatic;
         //Single subtotals: Sum
         //rowField.Subtotals = PivotFieldSubtotalType.Sum;
         //Multipl subtotals: Sum and count numbers 
         //rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

**Returns:**
int
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


Indique s'il faut afficher le sous‑total spécifié pour ce champ de tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Type de sous‑total. |

**Returns:**
booléen - Retourne si le sous‑total spécifié est affiché.
### getTop10AutoShowSettings() {#getTop10AutoShowSettings--}
```
public PivotFieldTop10AutoShowSettings getTop10AutoShowSettings()
```


Obtient les paramètres AutoShow du Top 10 pour un champ de tableau croisé dynamique.

**Returns:**
[PivotFieldTop10AutoShowSettings](../../com.aspose.cells/pivotfieldtop10autoshowsettings)
### group() {#group--}
```
public boolean group()
```


Regroupe automatiquement le champ.

**Remarks**

Si le champ ne contient que des valeurs vides et des dates, le champ sera groupé par mois. Si le champ ne contient que des valeurs vides et des nombres, le champ sera groupé par nombre. Sinon, il renvoie uniquement false sans aucun groupe.

**Returns:**
boolean
### group(PivotFieldGroupOptions options) {#group-com.aspose.cells.PivotFieldGroupOptions-}
```
public boolean group(PivotFieldGroupOptions options)
```


Regroupe le champ de tableau croisé dynamique avec des options.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [PivotFieldGroupOptions](../../com.aspose.cells/pivotfieldgroupoptions) | Options pour les paramètres de groupement du champ de tableau croisé dynamique. |

**Returns:**
boolean -
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Regroupe le fichier par les types de groupe de dates.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions) method . Cette méthode sera supprimée 6 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isAutoStart | boolean | Indique si la valeur de date/heure de début doit être détectée automatiquement. |
| start | [DateTime](../../com.aspose.cells/datetime) | La date/heure de début |
| isAutoEnd | boolean | Indique si la valeur de date/heure de fin doit être détectée automatiquement. |
| end | [DateTime](../../com.aspose.cells/datetime) | La date/heure de fin |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Types de groupe |
| intervalle | double | L'intervalle |
| firstAsNewField | boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé. Uniquement pour le premier élément du groupe. |

**Returns:**
booléen - False signifie que ce champ ne peut pas être groupé par date et heure.
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


Regroupe le fichier par numéro.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions) method . Cette méthode sera supprimée 6 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isAutoStart | boolean | Indique si la valeur de départ doit être détectée automatiquement. |
| début | double | La valeur de départ |
| isAutoEnd | boolean | Indique si la valeur de fin doit être détectée automatiquement. |
| fin | double | La fin de la valeur |
| intervalle | double | L'intervalle |
| newField | boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé |

**Returns:**
booléen - False signifie que ce champ ne peut pas être groupé par date et heure.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


Regroupe le champ de manière personnalisée.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions options) avec la propriété PivotFieldGroupOptions.DiscreteGroupItems. Cette méthode sera supprimée 6 mois plus tard, à partir de juillet 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | Les éléments de groupe personnalisés. |
| newField | boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé |

**Returns:**
booléen - False signifie que ce champ ne peut pas être groupé par date et heure.
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Regroupe le fichier par les types de groupe de dates.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions) method . Cette méthode sera supprimée 6 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | La date/heure de début |
| end | [DateTime](../../com.aspose.cells/datetime) | La date/heure de fin |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Types de groupe |
| intervalle | double | L'intervalle |
| firstAsNewField | boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé. Uniquement pour le premier élément du groupe. |

**Returns:**
booléen - False signifie que ce champ ne peut pas être groupé par date et heure.
### groupBy(DiscreteGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-}
```
public boolean groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)
```


Regroupe le champ de manière personnalisée.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions options) avec la propriété PivotFieldGroupOptions.DiscreteGroupItems. Cette méthode sera supprimée 6 mois plus tard, à partir de juillet 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| customGroupItems | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) | Les éléments de groupe personnalisés. |
| newField | boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé |

**Returns:**
boolean -
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


Regroupe automatiquement le champ avec un intervalle

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions) method . Cette méthode sera supprimée 6 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| intervalle | double | L'interne du groupe. Une valeur automatique sera assignée si elle est zéro, |
| newField | boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé. Seulement pour le groupe DateTime. |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


Regroupe le fichier par numéro.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions) method . Cette méthode sera supprimée 6 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | double | La valeur de départ |
| fin | double | La fin de la valeur |
| intervalle | double | L'intervalle |
| newField | boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé |

**Returns:**
booléen - False signifie que ce champ ne peut pas être groupé par date et heure.
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


Regroupe automatiquement le champ avec interne

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions) method . Cette méthode sera supprimée 6 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Types de groupe |
| intervalle | double | L'interne du groupe. Une valeur automatique sera assignée si elle est zéro, cela ne fonctionne que pour le regroupement par Nombres ou Jours. |
| newField | boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetails() {#hideAllDetails--}
```
public void hideAllDetails()
```


Masque tous les détails de chaque élément de tableau croisé dynamique.

### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


Définit si le détail de tous les PivotItems d'un champ de tableau croisé dynamique est masqué. C’est-à-dire réduire/étendre ce champ.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser les méthodes PivotItemsCollection.HideAllDetails() et UnhideAllDetails(). Cette méthode sera supprimée 12 mois plus tard, à partir de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isHiddenDetail | boolean | Indique si le détail du champ pivot doit être masqué. |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


Définit si l'élément PivotItem spécifique d'un champ de données est masqué.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.PivotItems[int].IsHidden. Cette méthode sera supprimée 12 mois plus tard, à partir d'août 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l'index du pivotItem dans le pivotField. |
| isHidden | boolean | si le PivotItem spécifique est masqué |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


Définit si l'élément PivotItem spécifique d'un champ de données est masqué.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.PivotItems[string].IsHidden. Cette méthode sera supprimée 12 mois plus tard, à partir d'août 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| itemValue | java.lang.String | Le nom du pivotItem dans le pivotField. |
| isHidden | boolean | Si le PivotItem spécifique est masqué |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


Définit si le détail de l'élément PivotItem spécifique d'un champ de tableau croisé dynamique est masqué.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.PivotItems[int].IsDetailHidden. Cette méthode sera supprimée 12 mois plus tard, à partir d'août 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l'index du pivotItem dans le pivotField. |
| isHiddenDetail | boolean | si le PivotItem spécifique est masqué |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


Initialise les éléments de tableau croisé dynamique du champ.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. Veuillez simplement supprimer l'appel à cette méthode. Cette méthode sera supprimée 6 mois plus tard, à partir d'octobre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement en ordre croissant.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.Top10AutoShowSettings.IsTop ou la méthode PivotField.Top10AutoShow(). Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


Indique si les éléments de ce champ de tableau croisé dynamique sont automatiquement triés par ordre croissant.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.SortSetting.SortType ou la méthode PivotField.SortBy(). Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.Top10AutoShowSettings.IsAutoShow ou la méthode PivotField.Top10AutoShow(). Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


Indique si les éléments de ce champ de tableau croisé dynamique sont triés automatiquement.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.SortSetting.SortType ou la méthode PivotField.SortBy(). Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


Indique si le champ spécifié affiche des sous‑totaux automatiques. La valeur par défaut est true.

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


Indique si ce champ de tableau croisé dynamique est un champ calculé.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


Indique si l'élément PivotItem spécifique est masqué.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.PivotItems[int].IsHidden. Cette méthode sera supprimée 12 mois plus tard, à partir d'août 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index du pivotItem dans le pivotField. |

**Returns:**
booléen - indique si le PivotItem spécifique est masqué
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


Indique s'il faut masquer le détail de l'élément PivotItem spécifique..

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.PivotItems[int].IsDetailHidden. Cette méthode sera supprimée 12 mois plus tard, à partir d'août 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index du pivotItem dans le pivotField. |

**Returns:**
booléen - indique si le détail du PivotItem spécifique est masqué
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


Indique s'il faut inclure de nouveaux éléments dans le champ du filtre manuel. La valeur par défaut est false.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


Indique s'il faut insérer des sauts de page après chaque élément. La valeur par défaut est false.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


Indique si plusieurs éléments peuvent être sélectionnés dans le champ de page. La valeur par défaut est false.

**Remarks**

Uniquement pour les champs de page (filtre).

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


Indique s'il faut répéter les libellés du champ dans la région ligne ou colonne. La valeur par défaut est false.

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


Indique si ce champ représente des champs de valeurs.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.IsValuesField. Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2023. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


Indique si ce champ représente un champ de valeurs.

**Remarks**

Fonctionne uniquement lorsqu'il y a deux champs de données ou plus dans la vue du tableau croisé dynamique.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllowDraggingToColumn(boolean value) {#setAllowDraggingToColumn-boolean-}
```
public void setAllowDraggingToColumn(boolean value)
```


Indique si le champ spécifié peut être glissé vers la région colonne. La valeur par défaut est vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowDraggingToData(boolean value) {#setAllowDraggingToData-boolean-}
```
public void setAllowDraggingToData(boolean value)
```


Indique si le champ spécifié peut être glissé vers la région valeurs. La valeur par défaut est vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowDraggingToPage(boolean value) {#setAllowDraggingToPage-boolean-}
```
public void setAllowDraggingToPage(boolean value)
```


Indique si le champ spécifié peut être glissé vers la région page. La valeur par défaut est vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowDraggingToRow(boolean value) {#setAllowDraggingToRow-boolean-}
```
public void setAllowDraggingToRow(boolean value)
```


Indique si le champ spécifié peut être glissé vers la région ligne. La valeur par défaut est vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowRemovingFromView(boolean value) {#setAllowRemovingFromView-boolean-}
```
public void setAllowRemovingFromView(boolean value)
```


Indique si ce champ de tableau croisé dynamique peut être supprimé de la vue du tableau croisé dynamique. La valeur par défaut est vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement en ordre croissant.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.Top10AutoShowSettings.IsTop ou la méthode PivotField.Top10AutoShow(). Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


Indique si les éléments de ce champ de tableau croisé dynamique sont automatiquement triés par ordre croissant.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.SortSetting.SortType ou la méthode PivotField.SortBy(). Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.Top10AutoShowSettings.IsAutoShow ou la méthode PivotField.Top10AutoShow(). Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ de tableau croisé dynamique spécifié.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.Top10AutoShowSettings.AutoShowCount ou la méthode PivotField.Top10AutoShow(). Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


Représente l'index du champ d'affichage automatique. -1 signifie le PivotField lui‑même. Il doit s'agir de l'index des champs de données.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.Top10AutoShowSettings.RankBy ou la méthode PivotField.Top10AutoShow(). Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


Indique si les éléments de ce champ de tableau croisé dynamique sont triés automatiquement.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.SortSetting.SortType ou la méthode PivotField.SortBy(). Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Représente l'index du champ qui est trié automatiquement. -1 signifie le PivotField lui‑même, les autres valeurs indiquent la position des champs de données.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.SortSetting.SortBy ou la méthode PivotField.SortBy(). Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


Indique si le champ spécifié affiche des sous‑totaux automatiques. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Représente l'index dans les champs pivot source.

**Remarks**

NOTE : Le mutateur de cette propriété est maintenant obsolète. Ce mutateur sera supprimé 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Définit l'élément de page actuellement affiché pour ce champ de tableau croisé dynamique (champ de page uniquement).

**Remarks**

Utilisez [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) comme valeur sentinelle pour indiquer "Select All". Il s'agit d'un marqueur prédéfini et ce n'est pas un index d'élément valide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short |  |

### setCurrentPageItemText(String value) {#setCurrentPageItemText-java.lang.String-}
```
public void setCurrentPageItemText(String value)
```


Obtient le texte d'affichage de l'élément de page actuel pour ce champ de tableau croisé dynamique (champ de page uniquement).

**Remarks**

Renvoie "(All)" lorsque [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--) est égal à [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX). Pour les autres valeurs, renvoie la représentation sous forme de chaîne de l'index de l'élément.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Représente le nom d'affichage du champ de tableau croisé dynamique dans la vue du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


Indique si le champ spécifié peut être glissé vers la région colonne. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToColumn. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


Indique si le champ spécifié peut être glissé vers la région valeurs. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToData. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Indique si ce champ de tableau croisé dynamique peut être supprimé de la vue du tableau croisé dynamique. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowRemovingFromView. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


Indique si le champ spécifié peut être glissé vers la région page. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToPage. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


Indique si le champ spécifié peut être glissé vers la région ligne. La valeur par défaut est vraie.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToRow. Cette méthode sera supprimée 12 mois plus tard, à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Représente la fonction utilisée pour résumer ce champ de données du tableau croisé dynamique.

Voir [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


Indique s'il faut inclure de nouveaux éléments dans le champ du filtre manuel. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Indique s'il faut insérer une ligne vide après chaque élément. Seulement pour les champs de ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


Indique s'il faut insérer des sauts de page après chaque élément. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


Indique si plusieurs éléments peuvent être sélectionnés dans le champ de page. La valeur par défaut est false.

**Remarks**

Uniquement pour les champs de page (filtre).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Représente le nom de PivotField.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


Indique si une opération de tri qui sera appliquée à ce champ de tableau croisé dynamique est une opération de tri automatique ou un tri de données simple.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété !PivotField.SortSetting.IsSimpleSort. Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Représente le format d'affichage intégré des nombres et des dates.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Représente le format d'affichage personnalisé des nombres et des dates.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


Indique s'il faut répéter les libellés du champ dans la région ligne ou colonne. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Indique si tous les éléments doivent être affichés dans la vue du tableau croisé dynamique, même s'ils ne contiennent pas de données récapitulatives. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Indique si les étiquettes du champ suivant doivent être affichées dans la même colonne dans la vue du tableau croisé dynamique. Uniquement pour les champs de ligne.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.ShowInCompactForm property instead . Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowInCompactForm(boolean value) {#setShowInCompactForm-boolean-}
```
public void setShowInCompactForm(boolean value)
```


Définit une valeur indiquant si ce champ de ligne utilise la disposition en forme compacte. S'applique uniquement aux champs de ligne.

**Remarks**

La forme compacte est un sous-mode de la disposition en plan. Ce paramètre ne prend effet que lorsque [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) est vrai.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Définit une valeur indiquant si ce champ de ligne utilise la disposition en plan. S'applique uniquement aux champs de ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


Indique s'il faut afficher les sous-totaux en haut ou en bas des éléments.

**Remarks**

Ne fonctionne que pour les champs de pivot dans la région des lignes lorsque ShowInOutlineForm est vrai.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSubtotals(int value) {#setSubtotals-int-}
```
public void setSubtotals(int value)
```


Définit les sous‑totaux du champ. Uniquement pour les champs de ligne ou de colonne du tableau croisé dynamique.

Voir [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Définit comment sous-totaliser le champ spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| affiché | boolean | Indique si le champ spécifié affiche ces sous‑totaux. |

### showAllDetails() {#showAllDetails--}
```
public void showAllDetails()
```


Afficher tous les détails de chaque élément de tableau croisé dynamique.

### showValuesAs(int showValuesAsType, int baseField, int baseItem) {#showValuesAs-int-int-int-}
```
public void showValuesAs(int showValuesAsType, int baseField, int baseItem)
```


Définit le calcul « Afficher les valeurs sous forme de » pour ce champ de tableau croisé dynamique.

**Remarks**

Uniquement pour le champ de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Type du calcul \"Afficher les valeurs comme\". |
| baseField | int | Index du champ de base utilisé pour le calcul. |
| baseItem | int | Index de l'élément de base utilisé pour le calcul. Utilisez [PivotShowValuesSetting.PREVIOUS\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#PREVIOUS-PIVOT-ITEM) (-1) pour l'élément précédent, [PivotShowValuesSetting.NEXT\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#NEXT-PIVOT-ITEM) (-2) pour l'élément suivant ; les valeurs non\\u9225\\u6182egatives désignent l'index ordinal d'un élément pivot spécifique. |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


Affiche les valeurs du champ de données dans un format d'affichage différent lorsque le calcul ShowDataAs est utilisé.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat). Le type de format d’affichage des données. |
| baseField | int | L’index du champ sur lequel le calcul ShowDataAs se base. |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype). Le type de position de l’élément de base. |
| baseItem | int | L’index de l’élément de base sur lequel le calcul ShowDataAs se base. Fonctionne uniquement lorsque baseItemPositionType est personnalisé. |

### showValuesAs(int showValuesAsType, String baseField, String baseItem) {#showValuesAs-int-java.lang.String-java.lang.String-}
```
public void showValuesAs(int showValuesAsType, String baseField, String baseItem)
```


Configure le calcul « Afficher les valeurs sous forme de » pour ce champ de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Le type de calcul pour Show Values As. |
| baseField | java.lang.String | Le nom du champ de base utilisé dans le calcul. |
| baseItem | java.lang.String | Légende d’un élément de tableau croisé dynamique ordinaire. Accepte également les mots-clés littéraux réservés : `(previous)` pour l’élément précédent, `(next)` pour l’élément suivant. Passez `null` si le type de calcul sélectionné ne nécessite pas d’élément de base. |

### sortBy(int sortType) {#sortBy-int-}
```
public void sortBy(int sortType)
```


Trie ce champ de tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Le type de tri de ce champ. |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


Trie ce champ de tableau croisé dynamique.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.SortBy(SortOrder, int,string) ou la propriété PivotField.IsAutoSort. Cette méthode sera supprimée 12 mois après septembre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Le type de tri de ce champ. |
| fieldSortedBy | int | L’index du champ de tableau croisé dynamique utilisé pour le tri. -1 signifie le tri par les étiquettes de données de ce champ, les autres valeurs indiquent l’index du champ de données utilisé pour le tri. |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


Trie ce champ de tableau croisé dynamique.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.SortBy(SortOrder, int,string). Cette méthode sera supprimée 12 mois après septembre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Le type de tri de ce champ. |
| fieldSortedBy | int | L’index du champ de tableau croisé dynamique utilisé pour le tri. -1 signifie le tri par les étiquettes de données de ce champ, les autres valeurs indiquent l’index du champ de données utilisé pour le tri. |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype). Le type de données triées par. |
| cellName | java.lang.String | Trier par valeurs dans la ligne ou la colonne |

### sortBy(int sortType, int fieldSortedBy, String cellName) {#sortBy-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, String cellName)
```


Trie ce champ de tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Le type de tri de ce champ. |
| fieldSortedBy | int | L’index du champ de tableau croisé dynamique utilisé pour le tri. -1 signifie le tri par les étiquettes de données de ce champ, les autres valeurs indiquent l’index du champ de données utilisé pour le tri. |
| cellName | java.lang.String | Trier par valeurs dans la ligne ou la colonne. Si Null, regrouper par le total du champ, sinon regrouper par les valeurs de la colonne ou ligne sélectionnée. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy) {#top10AutoShow-boolean-boolean-int-int-}
```
public void top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)
```


Configure les paramètres Top10 AutoShow pour ce champ de tableau croisé dynamique.

**Remarks**

Cette méthode configure le format binaire .XLS : AutoShow (Top10) est l’option native et la seule prise en charge. XLSX (OpenXML) : le format de fichier sous‑jacent prend en charge AutoShow Top10, mais l’interface utilisateur d’Excel 2007 et ultérieure ne l’expose que via le filtre Top10. Si la compatibilité XLS n’est pas requise, il est recommandé d’utiliser le filtre Top10 à la place.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isAutoShow | boolean | true pour activer AutoShow ; false pour le désactiver. |
| isTop | boolean | Si true, affiche les éléments supérieurs ; false affiche les éléments inférieurs. |
| count | int | Nombre d’éléments supérieurs/inférieurs à afficher. |
| rankBy | int | Index du champ de données utilisé pour le classement. Utilisez -1 pour classer par les propres valeurs de l’élément de tableau croisé dynamique. |

### ungroup() {#ungroup--}
```
public void ungroup()
```


Dégrouper le champ de tableau croisé dynamique.

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

