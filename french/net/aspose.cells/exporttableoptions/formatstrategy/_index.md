---
title: "ExportTableOptions.FormatStrategy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportTableOptions. Obtient et définit la stratégie de format lors de l'exportation de la valeur en tant que chaîne de caractères"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/formatstrategy/
---
## ExportTableOptions.FormatStrategy property

Obtient et définit la stratégie de format lors de l'exportation de la valeur en tant que chaîne.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Remarques

La valeur par défaut est CellStyle.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec mise en forme
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            Style styleB2 = worksheet.Cells["B2"].GetStyle();
            styleB2.Number = 4; // Currency format
            worksheet.Cells["B2"].SetStyle(styleB2);
            
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(599.99);
            Style styleB3 = worksheet.Cells["B3"].GetStyle();
            styleB3.Number = 4; // Currency format
            worksheet.Cells["B3"].SetStyle(styleB3);

            // Créer des options d'exportation avec différentes stratégies de format
            ExportTableOptions optionsDisplayStyle = new ExportTableOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                ExportColumnName = true
            };

            ExportTableOptions optionsCellStyle = new ExportTableOptions
            {
                FormatStrategy = CellValueFormatStrategy.CellStyle,
                ExportColumnName = true
            };

            // Exporter en utilisant différentes stratégies
            Console.WriteLine("DisplayStyle Format Strategy:");
            DataTable dtDisplay = worksheet.Cells.ExportDataTable(0, 0, 3, 2, optionsDisplayStyle);
            PrintDataTable(dtDisplay);

            Console.WriteLine("\nCellStyle Format Strategy:");
            DataTable dtCellStyle = worksheet.Cells.ExportDataTable(0, 0, 3, 2, optionsCellStyle);
            PrintDataTable(dtCellStyle);
        }

        private static void PrintDataTable(DataTable dt)
        {
            foreach (DataRow row in dt.Rows)
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

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


