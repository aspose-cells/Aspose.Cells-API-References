---
title: "AutoFitterOptions.AutoFitMergedCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFitterOptions-egenskap. Anger om radens höjd automatiskt anpassas när cellerna är sammanslagna i en rad. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

Anger om radens höjd automatiskt anpassas när cellerna är sammanslagna i en rad. Standardvärdet är false.

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället AutoFitterOptions.AutoFitMergedCellsType-egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan december 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata och slå samman celler
            worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
            worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3

            // Skapa AutoFitterOptions och sätt AutoFitMergedCells
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;

            // AutoFit rader med sammanslagna celler
            worksheet.AutoFitRows(options);

            // Spara arbetsboken
            workbook.Save("AutoFitMergedCellsExample.xlsx");
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


