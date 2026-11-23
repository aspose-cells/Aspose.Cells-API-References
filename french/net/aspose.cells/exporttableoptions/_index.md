---
title: "Classe ExportTableOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ExportTableOptions. Représente toutes les options d'exportation de tableau"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/
---
## ExportTableOptions class

Représente toutes les options d'exportation de tableau.

```csharp
public class ExportTableOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ExportTableOptions](exporttableoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AllowDBNull](../../aspose.cells/exporttableoptions/allowdbnull/) { get; set; } | Cette valeur indique si les DBNull sont autorisés dans ce tableau. |
| [CheckMixedValueType](../../aspose.cells/exporttableoptions/checkmixedvaluetype/) { get; set; } | False, Aspose.Cells définira le type du DataColumn en fonction du type de valeur de la première ligne pour des raisons de performance. True, Aspose.Cells vérifiera si le type de valeur dans la colonne est mixte avant de définir le type du DataColumn. Si les types de valeur sont mixtes, le type du DataColumn sera string. |
| [DataTable](../../aspose.cells/exporttableoptions/datatable/) { get; set; } | Obtient et définit le DataTable auquel le type de données des colonnes est attribué. |
| [ExportAsHtmlString](../../aspose.cells/exporttableoptions/exportashtmlstring/) { get; set; } | Exporte la valeur de chaîne HTML des cellules vers le DataTable. |
| [ExportAsString](../../aspose.cells/exporttableoptions/exportasstring/) { get; set; } | Exporte la valeur de chaîne des cellules vers le DataTable. |
| [ExportColumnName](../../aspose.cells/exporttableoptions/exportcolumnname/) { get; set; } | Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. La valeur par défaut est false. |
| [FormatStrategy](../../aspose.cells/exporttableoptions/formatstrategy/) { get; set; } | Obtient et définit la stratégie de format lors de l'exportation de la valeur en tant que chaîne. |
| [Indexes](../../aspose.cells/exporttableoptions/indexes/) { get; set; } | Les index des colonnes/lignes qui doivent être exportés. |
| [IsVertical](../../aspose.cells/exporttableoptions/isvertical/) { get; set; } | True si une ligne du fichier Workbook représente une ligne dans le DataTable. False si une colonne du fichier Workbook représente une ligne dans le DataTable. |
| [PlotVisibleCells](../../aspose.cells/exporttableoptions/plotvisiblecells/) { get; set; } | Exporte uniquement les cellules visibles. |
| [PlotVisibleColumns](../../aspose.cells/exporttableoptions/plotvisiblecolumns/) { get; set; } | Exporte uniquement les colonnes visibles. |
| [PlotVisibleRows](../../aspose.cells/exporttableoptions/plotvisiblerows/) { get; set; } | Exporte uniquement les lignes visibles. |
| [RenameStrategy](../../aspose.cells/exporttableoptions/renamestrategy/) { get; set; } | Stratégie pour les noms de colonnes en double. |
| [SkipErrorValue](../../aspose.cells/exporttableoptions/skiperrorvalue/) { get; set; } | Indique s'il faut ignorer les valeurs invalides pour la colonne. Par exemple, si le type de la colonne est décimal, que la valeur dépasse decimal.MaxValue et que cette propriété est true, nous ne lancerons plus d'exception. La valeur par défaut est false. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [PreprocessExportedValue](../../aspose.cells/exporttableoptions/preprocessexportedvalue/)(int, int, CellValue) | Prétraitez la valeur de la cellule actuelle à exporter. |

### Remarques

S'il existe des exigences particulières concernant l'exportation, comme ignorer les valeurs d'erreur, l'utilisateur peut étendre cette classe pour remplacer les API correspondantes afin d'atteindre l'objectif.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ExportTableOptionsDemo
    {
        public static void ExportTableOptionsExample()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells[0, 0].PutValue("Name");
            worksheet.Cells[0, 1].PutValue("Age");
            worksheet.Cells[1, 0].PutValue("John");
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue("Jane");
            worksheet.Cells[2, 1].PutValue(25);

            // Créez une instance de ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                SkipErrorValue = true,
                PlotVisibleCells = true,
                PlotVisibleRows = true,
                PlotVisibleColumns = true,
                ExportAsString = false,
                ExportAsHtmlString = false,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                CheckMixedValueType = true,
                AllowDBNull = true,
                IsVertical = true,
                RenameStrategy = RenameStrategy.Digit
            };

            // Exportez les données de la feuille de calcul vers un DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Afficher les données exportées
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Enregistrez le classeur
            workbook.Save("ExportTableOptionsExample.xlsx");
            workbook.Save("ExportTableOptionsExample.pdf");
        }
    }

}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


