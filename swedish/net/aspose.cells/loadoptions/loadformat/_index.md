---
title: "LoadOptions.LoadFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Hämtar inläsningsformatet"
type: docs
url: /sv/net/aspose.cells/loadoptions/loadformat/
---
## LoadOptions.LoadFormat property

Hämtar laddningsformatet.

```csharp
public LoadFormat LoadFormat { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Skapa exempel CSV-fil
            File.WriteAllText("sample.csv", "Name,Age\nJohn,30\nAlice,25");

            // Skapa LoadOptions för CSV-format och visa egenskapen
            LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
            Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

            // Läs in CSV med korrekta alternativ
            Workbook csvWorkbook = new Workbook("sample.csv", csvOptions);
            Console.WriteLine("CSV loaded cells: " + csvWorkbook.Worksheets[0].Cells["B1"].Value);

            // Skapa LoadOptions för XLSX-format och visa egenskapen
            LoadOptions xlsxOptions = new LoadOptions(LoadFormat.Xlsx);
            Console.WriteLine("\nXLSX LoadFormat: " + xlsxOptions.LoadFormat);

            // Skapa/spara exempel XLSX-fil
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Cells["A1"].PutValue("XLSX LoadFormat demo");
            newWorkbook.Save("sample.xlsx");

            // Läs in XLSX med korrekta alternativ
            Workbook xlsxWorkbook = new Workbook("sample.xlsx", xlsxOptions);
            Console.WriteLine("XLSX loaded cell: " + xlsxWorkbook.Worksheets[0].Cells["A1"].Value);

            // Rensa temporära filer
            File.Delete("sample.csv");
            File.Delete("sample.xlsx");
        }
    }
}
```

### Se även

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


