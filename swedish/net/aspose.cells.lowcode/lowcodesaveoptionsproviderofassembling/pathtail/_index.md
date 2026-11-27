---
title: "LowCodeSaveOptionsProviderOfAssembling.PathTail"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling-egenskap. Efterföljande del efter sekvensnummer i filvägen. Den bör inkludera filnamnets filändelse"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/
---
## LowCodeSaveOptionsProviderOfAssembling.PathTail property

Avslutningsdel (efter sekvensnummer) av filsökvägen. Den bör inkludera filnamnstillägget.

```csharp
public string PathTail { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathTailDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Record {i + 1}";
            }

            // Initiera sparalternativsleverantör
            var optionsProvider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SalesReports/Q3",
                PathTail = ".xlsx",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions
                {
                    SaveFormat = SaveFormat.Xlsx
                }
            };

            Console.WriteLine($"Original file extension: {optionsProvider.PathTail}");

            // Första sparandet med standardfiländelse
            workbook.Save("output_original", optionsProvider.SaveOptionsTemplate.SaveFormat);

            // Ändra filvägens svans för CSV-utdata
            optionsProvider.PathTail = "_split.csv";
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Csv;
            Console.WriteLine($"Modified file extension: {optionsProvider.PathTail}");

            // Andra sparandet med ny filändelse
            workbook.Save("output_modified", optionsProvider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check output directories for generated file formats");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


