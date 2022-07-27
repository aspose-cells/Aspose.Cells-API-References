---
title: GlobalizationSettings
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente les paramètres de globalisation.
type: docs
weight: 3620
url: /fr/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Représente les paramètres de globalisation.

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings) { get; set; } | Obtient ou définit le graphique de ce[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray) { get; } | Obtient le séparateur pour les éléments des données de ligne du tableau dans la formule. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator) { get; } | Obtient le séparateur pour la liste, les paramètres de la fonction, ...etc. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray) { get; } | Obtient le séparateur pour les lignes dans les données du tableau dans la formule. |

## Méthodes

| Nom | La description |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare)(string, string, bool) | Compare deux valeurs de chaîne selon certaines règles de classement. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname)() | Obtient le nom de l'étiquette "(Tous)" dans le tableau croisé dynamique. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring)(bool) | Obtient la valeur de la chaîne d'affichage pour la valeur booléenne de la cellule |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey)(string, bool) | Transforme la chaîne en un objet comparable selon certaines règles de classement. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable)() | Obtient le nom de l'étiquette "Column Labels" dans le tableau croisé dynamique. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename)(CommentTitleType) | Obtient le nom du titre du commentaire dépendant des paramètres régionaux en fonction du type de titre du commentaire. |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname)() | Obtient le nom de l'étiquette "(vide)" dans le tableau croisé dynamique. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring)(string) | Obtient la valeur de la chaîne d'affichage pour la valeur d'erreur de la cellule |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname)(ConsolidationFunction) | Obtient le nom du total général de la fonction. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname)(string) | Obtient le texte dépendant des paramètres régionaux pour le nom intégré en fonction du texte standard donné. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname)(string) | Obtient le nom de la fonction dépendante des paramètres régionaux en fonction du nom de fonction standard donné. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname)() | Obtient le nom de l'étiquette "(Plusieurs éléments)" dans le tableau croisé dynamique. |
| virtual [GetOtherName](../../aspose.cells/globalizationsettings/getothername)() | Obtient le nom des étiquettes "Autre" pour les graphiques à secteurs. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname)() | Obtient le nom de l'étiquette "Grand Total" dans le tableau croisé dynamique. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname)() | Obtient le nom de l'étiquette "Total" dans le tableau croisé dynamique. Vous devez remplacer cette méthode lorsque le tableau croisé dynamique contient deux champs croisés dynamiques ou plus dans la zone de données. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable)() | Obtient le nom de la protection dans le tableau croisé dynamique. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable)() | Obtient le nom de l'étiquette "Row Labels" dans le tableau croisé dynamique. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname)(string) | Obtient le texte standard du nom intégré en fonction du texte dépendant des paramètres régionaux donné. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname)(string) | Obtient le nom de la fonction standard en fonction du nom de la fonction dépendant des paramètres régionaux. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename)(string) | Obtient le nom du style de police anglais standard (régulier, gras, italique) pour l'en-tête/le pied de page en fonction du nom du style de police des paramètres régionaux. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname)(PivotFieldSubtotalType) | Obtient le nom de[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype) tapez dans le tableau croisé dynamique. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall)() | Obtient le nom de type des lignes de la table qui se compose de toutes les lignes de la table référencée. La valeur par défaut est "All", donc dans la formule "#All" représente toutes les lignes de la table référencée. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent)() | Obtient le nom de type des lignes de table qui se compose de la ligne actuelle dans la table référencée. La valeur par défaut est "Cette ligne", donc dans la formule "#Cette ligne" représente la ligne actuelle dans la table référencée. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata)() | Obtient le nom de type des lignes de table qui se compose de la région de données de la table référencée. La valeur par défaut est "Data", donc dans la formule "#Data" représente la région de données de la table. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders)() | Obtient le nom du type des lignes du tableau qui se compose de l'en-tête du tableau. La valeur par défaut est "Headers", donc dans la formule "#Headers" représente l'en-tête du tableau. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals)() | Obtient le nom de type des lignes de table qui se compose de la ligne totale de la table référencée. La valeur par défaut est "Totals", donc dans la formule "#Totals" représente la ligne totale de la table référencée. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname)(ConsolidationFunction) | Obtient le nom total de la fonction. |

### Voir également

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
