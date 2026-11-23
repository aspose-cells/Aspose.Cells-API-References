---
title: "ExportTableOptions.PlotVisibleColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportTableOptions. Exporte uniquement les colonnes visibles"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/plotvisiblecolumns/
---
## ExportTableOptions.PlotVisibleColumns property

Exporte uniquement les colonnes visibles.

```csharp
public bool PlotVisibleColumns { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleColumnsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et masquer certaines colonnes
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["D1"].PutValue("Column4");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data{i-1}_1");
                worksheet.Cells[$"B{i}"].PutValue($"Data{i-1}_2");
                worksheet.Cells[$"C{i}"].PutValue($"Data{i-1}_3");
                worksheet.Cells[$"D{i}"].PutValue($"Data{i-1}_4");
            }
            
            // Masquer la colonne C
            worksheet.Cells.HideColumn(2);

            // Exporter les données avec PlotVisibleColumns défini sur true
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.PlotVisibleColumns = true;

            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 6, 4, options);
            
            // Afficher les résultats
            Console.WriteLine("Exported DataTable Columns:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.WriteLine(column.ColumnName);
            }
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


