---
title: "Classe ListObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Tables.ListObject. Représente un tableau dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells.tables/listobject/
---
## ListObject class

Représente une table dans une feuille de calcul.

```csharp
public class ListObject
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription/) { get; set; } | Obtient et définit la description alternative. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext/) { get; set; } | Obtient et définit le texte alternatif. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter/) { get; } | Obtient le filtre automatique de ce tableau. |
| [Comment](../../aspose.cells.tables/listobject/comment/) { get; set; } | Obtient et définit le commentaire du tableau. |
| [DataRange](../../aspose.cells.tables/listobject/datarange/) { get; } | Obtient la plage de données du tableau. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype/) { get; } | Obtient le type de source de données du tableau. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname/) { get; set; } | Obtient et définit le nom d'affichage du tableau. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn/) { get; } | Obtient la colonne de fin de la plage. |
| [EndRow](../../aspose.cells.tables/listobject/endrow/) { get; } | Obtient la ligne de fin de la plage. |
| [HasAutoFilter](../../aspose.cells.tables/listobject/hasautofilter/) { get; set; } | Indique si le filtre automatique est appliqué à ce tableau. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns/) { get; } | Obtient la liste [`ListColumn`](../listcolumn/) de ce tableau. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable/) { get; } | Obtient la QueryTable liée. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow/) { get; set; } | Obtient et définit si ce tableau affiche la ligne d'en-tête. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes/) { get; set; } | Indique si le formatage à bandes de colonnes est appliqué. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn/) { get; set; } | Indique si la première colonne du tableau a le style appliqué. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn/) { get; set; } | Indique si la dernière colonne du tableau a le style appliqué. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes/) { get; set; } | Indique si le formatage à bandes de lignes est appliqué. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals/) { get; set; } | Obtient et définit si ce TAble affiche la ligne de total. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn/) { get; } | Obtient la colonne de départ de la plage. |
| [StartRow](../../aspose.cells.tables/listobject/startrow/) { get; } | Obtient la ligne de départ de la plage. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename/) { get; set; } | Obtient et définit le nom du style du tableau. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype/) { get; set; } | Obtient et le style de tableau intégré. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap/) { get; } | Obtient un [`XmlMap`](./xmlmap/) utilisé pour cette liste. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange/)() | Applique le style de tableau à la plage. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange)() | Convertit le tableau en plage. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange_1)(TableToRangeOptions) | Convertit le tableau en plage. |
| [Filter](../../aspose.cells.tables/listobject/filter/)() | (**Obsolète.**) Filtrer le tableau. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula)(int, int, string) | Placez la formule dans la cellule du tableau. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula_1)(int, int, string, bool) | Placez la formule dans la cellule du tableau. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue)(int, int, object) | Placez la valeur dans la cellule. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue_1)(int, int, object, bool) | Placez la valeur dans la cellule. |
| [RemoveAutoFilter](../../aspose.cells.tables/listobject/removeautofilter/)() | Supprime le filtre automatique appliqué à ce tableau. |
| [Resize](../../aspose.cells.tables/listobject/resize/)(int, int, int, int, bool) | Redimensionne la plage de l'objet de liste. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname/)() | Met à jour le nom de toutes les colonnes de liste dans les cellules du tableau. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectDemo
    {
        public static void ListObjectExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplissez la feuille de calcul avec quelques données
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Ajoutez un ListObject (table) à la feuille de calcul
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Définir certaines propriétés du ListObject
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
            table.DisplayName = "SampleTable";
            table.Comment = "This is a sample table.";
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.ShowTableStyleRowStripes = true;
            table.ShowTableStyleColumnStripes = true;
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Enregistrez le classeur
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


