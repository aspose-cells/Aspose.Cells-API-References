---
title: "Classe PivotField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotField. Représente un champ dans un rapport de tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Représente un champ dans un rapport PivotTable.

```csharp
public class PivotField : IDisposable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AllowDraggingToColumn](../../aspose.cells.pivot/pivotfield/allowdraggingtocolumn/) { get; set; } | Indique si le champ spécifié peut être glissé vers la région des colonnes. La valeur par défaut est true. |
| [AllowDraggingToData](../../aspose.cells.pivot/pivotfield/allowdraggingtodata/) { get; set; } | Indique si le champ spécifié peut être glissé vers la région des valeurs. La valeur par défaut est true. |
| [AllowDraggingToPage](../../aspose.cells.pivot/pivotfield/allowdraggingtopage/) { get; set; } | Indique si le champ spécifié peut être glissé vers la région des pages. La valeur par défaut est true. |
| [AllowDraggingToRow](../../aspose.cells.pivot/pivotfield/allowdraggingtorow/) { get; set; } | Indique si le champ spécifié peut être glissé vers la région des lignes. La valeur par défaut est true. |
| [AllowRemovingFromView](../../aspose.cells.pivot/pivotfield/allowremovingfromview/) { get; set; } | Indique si ce champ de tableau croisé dynamique peut être supprimé de la vue du tableau croisé dynamique. La valeur par défaut est true. |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount/) { get; set; } | (**Obsolete.**) Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ PivotTable spécifié. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield/) { get; set; } | (**Obsolete.**) Représente l'index du champ d'affichage automatique. -1 signifie le PivotField lui‑même. Il doit être l'index des champs de données. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield/) { get; set; } | (**Obsolete.**) Représente l'index du champ qui est trié automatiquement. -1 signifie le PivotField lui‑même, les autres valeurs indiquent la position des champs de données. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex/) { get; set; } | Représente l'index dans les champs pivot source. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem/) { get; set; } | Obtient ou définit l'élément de page actuellement affiché pour ce champ pivot (champ de page uniquement). |
| [CurrentPageItemText](../../aspose.cells.pivot/pivotfield/currentpageitemtext/) { get; set; } | Obtient le texte affiché de l'élément de page actuel pour ce champ pivot (champ de page uniquement). |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname/) { get; set; } | Représente le nom d'affichage du champ pivot dans la vue du tableau croisé dynamique. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn/) { get; set; } | (**Obsolete.**) Indique si le champ spécifié peut être glissé vers la région des colonnes. La valeur par défaut est vraie. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata/) { get; set; } | (**Obsolete.**) Indique si le champ spécifié peut être glissé vers la région des valeurs. La valeur par défaut est vraie. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide/) { get; set; } | (**Obsolete.**) Indique si ce champ pivot peut être supprimé de la vue du tableau croisé dynamique. La valeur par défaut est vraie. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage/) { get; set; } | (**Obsolete.**) Indique si le champ spécifié peut être glissé vers la région des pages. La valeur par défaut est vraie. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow/) { get; set; } | (**Obsolete.**) Indique si le champ spécifié peut être glissé vers la région des lignes. La valeur par défaut est vraie. |
| [Function](../../aspose.cells.pivot/pivotfield/function/) { get; set; } | Représente la fonction utilisée pour résumer ce champ de données du tableau croisé dynamique. |
| [GroupSettings](../../aspose.cells.pivot/pivotfield/groupsettings/) { get; } | Obtient les paramètres de groupe du champ pivot. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow/) { get; set; } | Indique s'il faut insérer une ligne vide après chaque élément. Uniquement pour les champs de ligne. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow/) { get; set; } | (**Obsolete.**) Indique si le champ PivotTable spécifié est affiché automatiquement en ordre croissant. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort/) { get; set; } | (**Obsolete.**) Indique si les éléments de ce champ pivot sont triés automatiquement en ordre croissant. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow/) { get; set; } | (**Obsolete.**) Indique si le champ PivotTable spécifié est affiché automatiquement. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort/) { get; set; } | (**Obsolete.**) Indique si les éléments de ce champ PivotTable sont triés automatiquement. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals/) { get; set; } | Indique si le champ spécifié affiche des sous‑totaux automatiques. La valeur par défaut est vraie. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield/) { get; } | Indique si ce champ pivot est un champ calculé. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/) { get; set; } | Indique s'il faut inclure de nouveaux éléments dans le champ lors d'un filtre manuel. La valeur par défaut est fausse. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/) { get; set; } | Indique s'il faut insérer des sauts de page après chaque élément. La valeur par défaut est fausse. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/) { get; set; } | Indique si plusieurs éléments peuvent être sélectionnés dans le champ de page. La valeur par défaut est fausse. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels/) { get; set; } | Indique s'il faut répéter les libellés du champ dans la région des lignes ou des colonnes. La valeur par défaut est fausse. |
| [IsValueFields](../../aspose.cells.pivot/pivotfield/isvaluefields/) { get; } | (**Obsolete.**) Indique si ce champ représente des champs de valeurs. |
| [IsValuesField](../../aspose.cells.pivot/pivotfield/isvaluesfield/) { get; } | Indique si ce champ représente un champ de valeurs. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount/) { get; } | (**Obsolete.**) Obtient le nombre d'éléments de base dans ce champ pivot. |
| [Items](../../aspose.cells.pivot/pivotfield/items/) { get; } | Obtient toutes les étiquettes des éléments pivot dans ce champ. |
| [Name](../../aspose.cells.pivot/pivotfield/name/) { get; set; } | Représente le nom de PivotField. |
| [NonAutoSortDefault](../../aspose.cells.pivot/pivotfield/nonautosortdefault/) { get; set; } | (**Obsolete.**) Indique si une opération de tri qui sera appliquée à ce champ pivot est un tri automatique ou un tri de données simple. |
| [Number](../../aspose.cells.pivot/pivotfield/number/) { get; set; } | Représente le format d'affichage intégré des nombres et des dates. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat/) { get; set; } | Représente le format d'affichage personnalisé des nombres et des dates. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems/) { get; } | Obtient les éléments de base originaux; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems/) { get; } | Obtient les éléments pivot du champ pivot |
| [Position](../../aspose.cells.pivot/pivotfield/position/) { get; } | Représente l'index de `PivotField` dans la région. |
| [RegionType](../../aspose.cells.pivot/pivotfield/regiontype/) { get; } | Spécifie la région du tableau croisé dynamique où ce champ est affiché. |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems/) { get; set; } | Indique s'il faut afficher tous les éléments dans la vue du tableau croisé dynamique, même s'ils ne contiennent pas de données de synthèse. La valeur par défaut est false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact/) { get; set; } | (**Obsolete.**) Indique s'il faut afficher les étiquettes du champ suivant dans la même colonne dans la vue du tableau croisé dynamique. Seulement pour les champs de ligne. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivotfield/showincompactform/) { get; set; } | Obtient ou définit une valeur indiquant si ce champ de ligne utilise la disposition en forme compacte. S'applique uniquement aux champs de ligne. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform/) { get; set; } | Obtient ou définit une valeur indiquant si ce champ de ligne utilise la disposition en plan. S'applique uniquement aux champs de ligne. |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop/) { get; set; } | Indique s'il faut afficher les sous‑totaux en haut ou en bas des éléments. |
| [ShowValuesSetting](../../aspose.cells.pivot/pivotfield/showvaluessetting/) { get; } | Obtient les paramètres d'affichage des valeurs lorsque le calcul ShowDataAs est utilisé. |
| [SortSetting](../../aspose.cells.pivot/pivotfield/sortsetting/) { get; } | Obtient tous les paramètres du tri automatique |
| [Subtotals](../../aspose.cells.pivot/pivotfield/subtotals/) { get; set; } | Obtient ou définit les sous‑totaux du champ. Seulement pour les champs pivot de ligne ou de colonne. |
| [Top10AutoShowSettings](../../aspose.cells.pivot/pivotfield/top10autoshowsettings/) { get; } | Obtient les paramètres AutoShow Top 10 pour un champ pivot. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem/)(string, string) | Ajoute un élément de formule calculée au champ pivot. |
| [ClearFilter](../../aspose.cells.pivot/pivotfield/clearfilter/)() | Efface le paramètre de filtre sur ce champ pivot. |
| [Dispose](../../aspose.cells.pivot/pivotfield/dispose/)() | Effectue des tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [FilterByDate](../../aspose.cells.pivot/pivotfield/filterbydate/)(PivotFilterType, DateTime, DateTime) | Filtre par valeurs de date du champ pivot de ligne ou de colonne. |
| [FilterByLabel](../../aspose.cells.pivot/pivotfield/filterbylabel/)(PivotFilterType, string, string) | Filtre par légendes du champ pivot de ligne ou de colonne. |
| [FilterByValue](../../aspose.cells.pivot/pivotfield/filterbyvalue/)(int, PivotFilterType, double, double) | Filtre par valeurs du champ pivot de données. |
| [FilterTop10](../../aspose.cells.pivot/pivotfield/filtertop10/)(int, PivotFilterType, bool, int) | Filtre par valeurs du champ pivot de données. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula/)() | (**Obsolete.**) Obtient la chaîne de formule du champ calculé spécifié. |
| [GetFilters](../../aspose.cells.pivot/pivotfield/getfilters/)() | Obtient tous les filtres de tableau croisé dynamique appliqués à ce champ de tableau croisé dynamique. |
| [GetFormula](../../aspose.cells.pivot/pivotfield/getformula/)() | Obtient la formule du champ calculé. Fonctionne uniquement pour le champ calculé. |
| [GetMaxValue](../../aspose.cells.pivot/pivotfield/getmaxvalue/)() | Obtient la valeur maximale de ce champ. |
| [GetMinValue](../../aspose.cells.pivot/pivotfield/getminvalue/)() | Obtient la valeur maximale de ce champ. |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype/)(PivotFilterType) | Obtient le filtre de tableau croisé dynamique du champ de tableau croisé dynamique par type |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters/)() | (**Obsolete.**) Obtient les filtres de tableau croisé dynamique du champ de tableau croisé dynamique. |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals/)(PivotFieldSubtotalType) | Indique s’il faut afficher le sous‑total spécifié pour ce champ de tableau croisé dynamique. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group)() | Regroupe automatiquement le champ. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group_1)(PivotFieldGroupOptions) | Regroupe le champ de tableau croisé dynamique avec des options. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby)(CustomPiovtFieldGroupItem[], bool) | (**Obsolete.**) Regroupe le champ de manière personnalisée. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_1)(DiscreteGroupItem[], bool) | (**Obsolete.**) Regroupe le champ de manière personnalisée. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_7)(double, bool) | (**Obsolete.**) Regroupe automatiquement le champ avec un intervalle |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_6)(PivotGroupByType[], double, bool) | (**Obsolete.**) Regroupe automatiquement le champ avec interne |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_4)(double, double, double, bool) | (**Obsolete.**) Regroupe le fichier par numéro. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_5)(DateTime, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) Regroupe le fichier par les types de groupe de dates. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_2)(bool, double, bool, double, double, bool) | (**Obsolete.**) Regroupe le fichier par numéro. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_3)(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) Regroupe le fichier par les types de groupe de dates. |
| [HideAllDetails](../../aspose.cells.pivot/pivotfield/hidealldetails/)() | Masque tous les détails de chaque élément de tableau croisé dynamique. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail/)(bool) | (**Obsolete.**) Définit si le détail de tous les PivotItems d’un champ de tableau croisé dynamique est masqué. C’est‑à‑dire réduire/étendre ce champ. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem)(int, bool) | (**Obsolete.**) Définit si le PivotItem spécifique d’un champ de données est masqué. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem_1)(string, bool) | (**Obsolete.**) Définit si le PivotItem spécifique d’un champ de données est masqué. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail/)(int, bool) | (**Obsolete.**) Définit si le détail du PivotItem spécifique dans un champ de tableau croisé dynamique est masqué. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems/)() | (**Obsolete.**) Initialise les éléments de tableau croisé dynamique du champ de tableau croisé dynamique |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem/)(int) | (**Obsolete.**) Indique si le PivotItem spécifique est masqué. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail/)(int) | (**Obsolete.**) Indique s’il faut masquer le détail du PivotItem spécifique. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals/)(PivotFieldSubtotalType, bool) | Définit comment sous‑totaliser le champ spécifié. |
| [ShowAllDetails](../../aspose.cells.pivot/pivotfield/showalldetails/)() | Affiche tous les détails de chaque élément de tableau croisé dynamique. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_1)(PivotShowValuesAsType, int, int) | Définit le calcul "Show Values As" pour ce champ de tableau croisé dynamique. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_2)(PivotShowValuesAsType, string, string) | Configure le calcul "Show Values As" pour ce champ de données. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas)(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) | (**Obsolete.**) Affiche les valeurs du champ de données sous un format d’affichage différent lorsque le calcul ShowDataAs est utilisé. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby)(SortOrder) | Trie ce champ pivot. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_1)(SortOrder, int) | (**Obsolète.**) Trie ce champ pivot. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_3)(SortOrder, int, string) | Trie ce champ pivot. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_2)(SortOrder, int, PivotLineType, string) | (**Obsolète.**) Trie ce champ pivot. |
| [Top10AutoShow](../../aspose.cells.pivot/pivotfield/top10autoshow/)(bool, bool, int, int) | Configure les paramètres Top10 AutoShow pour ce champ pivot. |
| [Ungroup](../../aspose.cells.pivot/pivotfield/ungroup/)() | Dégrouper le champ pivot. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDemo
    {
        public static void PivotFieldExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajouter des données à la feuille de calcul
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "amount");

            // Définissez le style du tableau croisé dynamique
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Accédez au champ de ligne
            PivotField rowField = pivotTable.RowFields[0];

            // Définir les propriétés du PivotField
            rowField.DisplayName = "Custom Display Name";
            rowField.IsAutoSubtotals = false;
            rowField.DragToColumn = true;
            rowField.DragToHide = true;
            rowField.DragToRow = true;
            rowField.DragToPage = true;
            rowField.DragToData = true;
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.IsRepeatItemLabels = true;
            rowField.IsIncludeNewItemsInFilter = true;
            rowField.IsInsertPageBreaksBetweenItems = true;
            rowField.ShowAllItems = true;
            rowField.NonAutoSortDefault = true;
            rowField.IsAutoSort = true;
            rowField.IsAscendSort = true;
            rowField.AutoSortField = -1;
            rowField.IsAutoShow = true;
            rowField.IsAscendShow = true;
            rowField.AutoShowCount = 5;
            rowField.AutoShowField = -1;
            rowField.Function = ConsolidationFunction.Sum;
            rowField.ShowValuesAs(PivotFieldDataDisplayFormat.PercentageOfTotal, 0, PivotItemPositionType.Next, 0);
            rowField.CurrentPageItem = 1;
            rowField.Number = 0;
            rowField.InsertBlankRow = true;
            rowField.ShowSubtotalAtTop = true;
            rowField.ShowInOutlineForm = true;
            rowField.NumberFormat = "0.00";
            rowField.ShowCompact = true;

            // Actualiser et calculer les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotFieldExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


