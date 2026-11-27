---
title: "JsonSaveOptions.ExportStylePool"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Anger om stilar ska exporteras kollektivt eller individuellt till varje cell"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/exportstylepool/
---
## JsonSaveOptions.ExportStylePool property

Indikerar om stilar ska exporteras kollektivt eller individuellt till varje cell.

```csharp
public bool ExportStylePool { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertyExportStylePoolDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med olika stilar
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);

            // Applicera olika stilar på celler
            Aspose.Cells.Style style1 = workbook.CreateStyle();
            style1.Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(style1);

            Aspose.Cells.Style style2 = workbook.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Blue;
            worksheet.Cells["B1"].SetStyle(style2);

            try
            {
                // Skapa JsonSaveOptions med ExportStylePool = true (kollektiv export)
                JsonSaveOptions options1 = new JsonSaveOptions();
                options1.ExportStylePool = true;
                Console.WriteLine("ExportStylePool (collective): " + options1.ExportStylePool);

                // Spara med kollektiv stilexport
                workbook.Save("output_collective_styles.json", options1);

                // Skapa JsonSaveOptions med ExportStylePool = false (individuell export)
                JsonSaveOptions options2 = new JsonSaveOptions();
                options2.ExportStylePool = false;
                Console.WriteLine("ExportStylePool (individual): " + options2.ExportStylePool);

                // Spara med individuell stilexport
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

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


