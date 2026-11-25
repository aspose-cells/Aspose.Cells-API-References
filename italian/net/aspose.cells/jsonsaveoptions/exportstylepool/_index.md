---
title: "JsonSaveOptions.ExportStylePool"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Indica se esportare gli stili collettivamente o individualmente per ogni cella"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/exportstylepool/
---
## JsonSaveOptions.ExportStylePool property

Indica se esportare gli stili collettivamente o individualmente per ogni cella.

```csharp
public bool ExportStylePool { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertyExportStylePoolDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con stili diversi
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);

            // Applica stili diversi alle celle
            Aspose.Cells.Style style1 = workbook.CreateStyle();
            style1.Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(style1);

            Aspose.Cells.Style style2 = workbook.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Blue;
            worksheet.Cells["B1"].SetStyle(style2);

            try
            {
                // Crea JsonSaveOptions con ExportStylePool = true (esportazione collettiva)
                JsonSaveOptions options1 = new JsonSaveOptions();
                options1.ExportStylePool = true;
                Console.WriteLine("ExportStylePool (collective): " + options1.ExportStylePool);

                // Salva con esportazione di stile collettiva
                workbook.Save("output_collective_styles.json", options1);

                // Crea JsonSaveOptions con ExportStylePool = false (esportazione individuale)
                JsonSaveOptions options2 = new JsonSaveOptions();
                options2.ExportStylePool = false;
                Console.WriteLine("ExportStylePool (individual): " + options2.ExportStylePool);

                // Salva con esportazione di stile individuale
                workbook.Save("output_individual_styles.json", options2);

                Console.WriteLine("ExportStylePool demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


