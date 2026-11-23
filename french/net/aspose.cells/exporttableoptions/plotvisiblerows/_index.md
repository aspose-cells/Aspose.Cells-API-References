---
title: "ExportTableOptions.PlotVisibleRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ExportTableOptions property. N’exporte que les lignes visibles"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

Exporte uniquement les lignes visibles.

```csharp
public bool PlotVisibleRows { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleRowsDemo
    {
        public static void Run()
        {
            // Créer un classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer des données d'exemple dans la feuille de calcul
            cells["A1"].PutValue("Column1");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);
            cells["A4"].PutValue(30);

            // Masquer la ligne 3 (index 2) qui contient la valeur 20
            worksheet.Cells.HideRow(2);

            // Créer un DataTable vers lequel exporter
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Column1", typeof(int));

            // Configurer les options d'exportation
            ExportTableOptions options = new ExportTableOptions();
            options.PlotVisibleRows = true; // Only export visible rows
            options.ExportColumnName = true;
            options.DataTable = dataTable;

            // Exporter les données (devrait ignorer la ligne masquée)
            cells.ExportDataTable(0, 0, 4, 1, options);

            // Afficher les données exportées
            Console.WriteLine("Exported Data (PlotVisibleRows=true):");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine(row["Column1"]);
            }
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


