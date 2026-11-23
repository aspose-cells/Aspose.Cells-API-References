---
title: "ExportTableOptions.PlotVisibleCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ExportTableOptions property. N’exporte que les cellules visibles"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/plotvisiblecells/
---
## ExportTableOptions.PlotVisibleCells property

Exporte uniquement les cellules visibles.

```csharp
public bool PlotVisibleCells { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec certaines lignes/colonnes masquées
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");
            
            // Masquer la ligne 2 et la colonne B (index 1)
            worksheet.Cells.HideRow(1);
            worksheet.Cells.HideColumn(1);

            // Créer des options d'exportation avec PlotVisibleCells défini sur true
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                PlotVisibleCells = true,
                PlotVisibleColumns = true,
                PlotVisibleRows = true
            };

            // Exporter uniquement les cellules visibles
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 3, exportOptions);

            // Afficher les données exportées (seules les cellules visibles doivent être exportées)
            Console.WriteLine("Exported Data:");
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


