---
title: "Classe GlobalizationSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GlobalizationSettings class. Représente les paramètres de mondialisation"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Représente les paramètres de mondialisation.

```csharp
public class GlobalizationSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Obtient ou définit les paramètres de mondialisation pour le graphique. |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray/) { get; } | Obtient le séparateur des éléments dans les données de ligne du tableau dans la formule. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator/) { get; } | Obtient le séparateur pour les listes, les paramètres de fonction, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Obtient ou définit les paramètres de mondialisation pour le tableau croisé dynamique. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray/) { get; } | Obtient le séparateur des lignes dans les données de tableau dans la formule. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Compare deux valeurs de chaîne selon certaines règles de collation. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Obtient le nom de l'étiquette "(All)" dans le tableau croisé dynamique. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring/)(bool) | Obtient la chaîne d'affichage de la valeur booléenne de la cellule |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Transforme la chaîne en un objet comparable selon certaines règles de collation. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Obtient le nom de l'étiquette "Column Labels" dans le tableau croisé dynamique. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename/)(CommentTitleType) | Obtient le nom du titre du commentaire dépendant de la langue selon le type de titre de commentaire. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Obtient le nom de l’en-tête du champ de zone de valeurs dans le tableau croisé dynamique. |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Obtient le nom de feuille par défaut pour l’ajout automatique d’une feuille de calcul. La valeur par défaut est "Sheet". |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Obtient le nom de l’étiquette "(blank)" dans le tableau croisé dynamique. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring/)(string) | Obtient la chaîne d'affichage de la valeur d'erreur de la cellule |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Obtient le nom du total général de la fonction. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname/)(string) | Obtient le texte dépendant de la langue pour le nom intégré selon le texte standard fourni. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname/)(string) | Obtient le nom de fonction dépendant de la langue selon le nom de fonction standard fourni. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Obtient le nom de l’étiquette "(Multiple Items)" dans le tableau croisé dynamique. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Obtient le nom de l’étiquette "Grand Total" dans le tableau croisé dynamique. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Obtient le nom de l’étiquette "Total" dans le tableau croisé dynamique. Vous devez remplacer cette méthode lorsque le tableau croisé dynamique contient deux champs ou plus dans la zone de données. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Obtient le nom de la protection dans le tableau croisé dynamique. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Obtient le nom de l’étiquette "Row Labels" dans le tableau croisé dynamique. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname/)(string) | Obtient le texte standard du nom intégré selon le texte dépendant de la langue fourni. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname/)(string) | Obtient le nom de fonction standard selon le nom de fonction dépendant de la langue fourni. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/)(string) | Obtient le nom de style de police anglais standard (Regular, Bold, Italic) pour En-tête/Pied de page selon le nom de style de police dépendant de la langue fourni. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Obtient le nom du type [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) dans le tableau croisé dynamique. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall/)() | Obtient le nom du type de lignes de tableau qui comprend toutes les lignes du tableau référencé. La valeur par défaut est "All", ainsi dans la formule "#All" représente toutes les lignes du tableau référencé. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent/)() | Obtient le nom du type de lignes de tableau qui comprend la ligne actuelle du tableau référencé. La valeur par défaut est "This Row", ainsi dans la formule "#This Row" représente la ligne actuelle du tableau référencé. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata/)() | Obtient le nom du type des lignes de tableau qui comprend la région de données du tableau référencé. La valeur par défaut est "Data", donc dans la formule "#Data" représente la région de données du tableau. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders/)() | Obtient le nom du type des lignes de tableau qui comprend l'en-tête du tableau. La valeur par défaut est "Headers", donc dans la formule "#Headers" représente l'en-tête du tableau. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals/)() | Obtient le nom du type de lignes de tableau qui comprend la ligne totale du tableau référencé. La valeur par défaut est "Totals", ainsi dans la formule "#Totals" représente la ligne totale du tableau référencé. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname/)(ConsolidationFunction) | Obtient le nom total de la fonction. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple
            cells["A1"].PutValue("Region");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("North");
            cells["B2"].PutValue(1000);
            cells["A3"].PutValue("South");
            cells["B3"].PutValue(2000);
            cells["A4"].PutValue("East");
            cells["B4"].PutValue(3000);
            cells["A5"].PutValue("West");
            cells["B5"].PutValue(4000);

            // Créer et appliquer les paramètres de mondialisation
            GlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Appliquer le sous-total avec une mondialisation personnalisée
            CellArea area = CellArea.CreateCellArea(0, 0, 5, 1);
            cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 0 }, true, false, true);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTotalName(ConsolidationFunction functionType)
        {
            // Personnaliser le nom total en fonction du type de fonction
            switch (functionType)
            {
                case ConsolidationFunction.Sum:
                    return "Custom Sum";
                case ConsolidationFunction.Count:
                    return "Custom Count";
                default:
                    return base.GetTotalName(functionType);
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


