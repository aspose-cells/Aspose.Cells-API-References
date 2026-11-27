---
title: "Workbook.FileName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar och anger det aktuella filnamnet"
type: docs
url: /sv/net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Hämtar och anger det aktuella filnamnet.

```csharp
public string FileName { get; set; }
```

### Anmärkningar

Om filen öppnas via en ström och det finns externa formelreferenser, vänligen ange filnamnet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Ange filnamnsegenskapen
            wb.FileName = "SampleWorkbook.xlsx";
            
            // Lägg till lite data för att demonstrera funktionaliteten
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Workbook FileName Demo");
            sheet.Cells["A2"].PutValue("Current FileName:");
            sheet.Cells["B2"].PutValue(wb.FileName);
            
            // Spara arbetsboken
            wb.Save(wb.FileName);
            
            Console.WriteLine($"Workbook created with filename: {wb.FileName}");
            
            // Demonstrera ändring av filnamnet
            Workbook wb2 = new Workbook();
            wb2.FileName = "ChangedName.xlsx";
            Console.WriteLine($"New workbook filename set to: {wb2.FileName}");
            
            // Demonstrera användning av externa länkar
            if (wb.Worksheets.ExternalLinks.Count > 0)
            {
                string externalSource = wb.Worksheets.ExternalLinks[0].DataSource;
                wb2.FileName = externalSource;
                Console.WriteLine($"Updated filename to external source: {wb2.FileName}");
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


