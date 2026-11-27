---
title: "SaveOptions.MergeAreas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Anger om områdena för villkorsstyrd formatering och validering ska slås samman innan filen sparas"
type: docs
url: /sv/net/aspose.cells/saveoptions/mergeareas/
---
## SaveOptions.MergeAreas property

Anger om områdena för villkorsstyrd formatering och validering ska slås samman innan filen sparas.

```csharp
public bool MergeAreas { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyMergeAreasDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i data och skapa sammanslagna celler
            worksheet.Cells["A1"].PutValue("Merged Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Slå samman celler A1:B1
            worksheet.Cells.Merge(0, 0, 1, 2);

            // Skapa sparaalternativ med MergeAreas aktiverat
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MergeAreas = true;

            // Spara med optimering av sammanslagna områden
            workbook.Save("MergeAreasDemo.xlsx", saveOptions);
        }
    }
}
```

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


