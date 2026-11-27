---
title: "SaveOptions.ValidateMergedAreas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Anger om sammanslagna celler ska valideras innan filen sparas"
type: docs
url: /sv/net/aspose.cells/saveoptions/validatemergedareas/
---
## SaveOptions.ValidateMergedAreas property

Anger om sammanslagna celler ska valideras innan filen sparas.

```csharp
public bool ValidateMergedAreas { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyValidateMergedAreasDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange värden och slå samman celler
            worksheet.Cells["A1"].PutValue("Merged Area");
            worksheet.Cells["A2"].PutValue("Test");
            worksheet.Cells.Merge(0, 0, 2, 1); // Merge A1:A2

            // Skapa sparalternativ med ValidateMergedAreas satt till true
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                ValidateMergedAreas = true,
                MergeAreas = true
            };

            // Spara arbetsboken med validering av sammanslagna områden
            workbook.Save("ValidateMergedAreasDemo.xlsb", saveOptions);

            Console.WriteLine("Workbook saved with merged areas validation.");
        }
    }
}
```

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


