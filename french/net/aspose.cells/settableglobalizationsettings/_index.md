---
title: "Classe SettableGlobalizationSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.SettableGlobalizationSettings class. Implémentation de GlobalizationSettings qui permet à l'utilisateur de définir/modifier les textes prédéfinis"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/
---
## SettableGlobalizationSettings class

Implémentation de GlobalizationSettings qui permet à l'utilisateur de définir/modifier des textes prédéfinis.

```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Obtient ou définit les paramètres de mondialisation pour Chart.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | Obtient le séparateur des éléments dans les données de ligne du tableau dans la formule. |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | Obtient le séparateur pour les listes, les paramètres de fonction, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Obtient ou définit les paramètres de mondialisation pour le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | Obtient le séparateur des lignes dans les données de tableau dans la formule. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Compare deux valeurs de chaîne selon certaines règles de collation.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Obtient le nom de l\u00e9tiquette "(All)" dans le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | Obtient la chaîne d'affichage de la valeur booléenne de la cellule |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Transforme la chaîne en un objet comparable selon certaines règles de collation.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Obtient le nom de l\u00e9tiquette "Column Labels" dans le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | Obtient le nom du titre du commentaire dépendant de la langue selon le type de titre de commentaire. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Obtient le nom de l'en-tête du champ de zone de valeur dans le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Obtient le nom de feuille par défaut pour l'ajout automatique d'une feuille de calcul. La valeur par défaut est "Sheet".(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Obtient le nom de l\u00e9tiquette "(blank)" dans le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | Obtient la chaîne d'affichage de la valeur d'erreur de la cellule |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Obtient le nom du total général de la fonction. |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | Obtient le texte dépendant de la langue pour le nom intégré selon le texte standard fourni. |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | Obtient le nom de fonction dépendant de la langue selon le nom de fonction standard fourni. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Obtient le nom de l\u00e9tiquette "(Multiple Items)" dans le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Obtient le nom de l\u00e9tiquette "Grand Total" dans le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Obtient le nom de l\u00e9tiquette "Total" dans le tableau croisé dynamique. Vous devez remplacer cette méthode lorsque le tableau croisé dynamique contient deux champs ou plus dans la zone de données.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Obtient le nom de la protection dans le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Obtient le nom de l\u00e9tiquette "Row Labels" dans le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | Obtient le texte standard du nom intégré selon le texte dépendant de la langue fourni. |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | Obtient le nom de fonction standard selon le nom de fonction dépendant de la langue fourni. |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | Obtient le nom de style de police anglais standard (Regular, Bold, Italic) pour En-tête/Pied de page selon le nom de style de police dépendant de la langue fourni. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Obtient le nom du type [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) dans le tableau croisé dynamique.(Hérité de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | Obtient le nom du type des lignes de tableau qui comprend toutes les lignes du tableau référencé. |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | Obtient le nom du type des lignes de tableau qui comprend la ligne actuelle du tableau référencé. |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | Obtient le nom du type des lignes de tableau qui comprend la région de données du tableau référencé. La valeur par défaut est "Data", donc dans la formule "#Data" représente la région de données du tableau. |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | Obtient le nom du type des lignes de tableau qui comprend l'en-tête du tableau. La valeur par défaut est "Headers", donc dans la formule "#Headers" représente l'en-tête du tableau. |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | Obtient le nom du type des lignes de tableau qui comprennent la ligne totale du tableau référencé. |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | Obtient le nom total de la fonction spécifique. |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | Définit la valeur de chaîne d'affichage pour la valeur booléenne de la cellule |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | Définit le séparateur pour les éléments des données de ligne du tableau dans la formule. |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | Obtient le nom du titre du commentaire dépendant de la langue selon le type de titre de commentaire. |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | Définit le nom du total général de la fonction spécifique. |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | Définit le séparateur pour la liste, les paramètres de la fonction, ...etc. |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | Définit le texte dépendant de la langue pour le nom intégré avec le texte du nom standard donné. |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | Définit le nom de fonction dépendant de la langue correspondant au nom de fonction standard donné. |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | Définit le séparateur pour les lignes des données de tableau dans la formule. |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | Définit le nom de fonction dépendant de la langue selon le nom de fonction standard donné. |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | Définit le nom de fonction dépendant de la langue selon le nom de fonction standard donné. |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | Définit le nom de fonction dépendant de la langue selon le nom de fonction standard donné. |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | Définit le nom du type des lignes de tableau qui comprennent toutes les lignes du tableau référencé. |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | Définit le nom du type des lignes de tableau qui comprennent la ligne actuelle du tableau référencé. |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | Définit le nom du type des lignes de tableau qui comprennent la région de données du tableau référencé. |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | Définit le nom du type des lignes de tableau qui comprennent l'en-tête du tableau. |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | Définit le nom du type des lignes de tableau qui comprennent la ligne totale du tableau référencé. |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | Définit le nom total de la fonction spécifique. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class CellsClassSettableGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Définir le séparateur de liste personnalisé
            settings.SetListSeparator(';');

            // Définir les chaînes de valeurs booléennes personnalisées
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Définir les noms de fonctions personnalisés
            settings.SetLocalFunctionName("SUM", "SUMME", true);
            settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);

            // Définir les noms de type de ligne de tableau personnalisés
            settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
            settings.SetTableRowTypeOfData("DATA_CUSTOM");
            settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");

            // Définir les noms de titre de commentaire personnalisés
            settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
            // Ligne Author supprimée car CommentTitleType ne possède pas cette valeur d'énumération
            // Si vous devez définir des paramètres liés à l'auteur, vous devez utiliser ThreadedCommentAuthor à la place

            // Appliquer les paramètres de globalisation au classeur
            workbook.Settings.GlobalizationSettings = settings;

            // Démontrer l'utilisation dans les formules
            worksheet.Cells["A1"].Formula = "=TRUE()";
            worksheet.Cells["A2"].Formula = "=FALSE()";
            worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
            worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";

            // Enregistrez le classeur
            workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


