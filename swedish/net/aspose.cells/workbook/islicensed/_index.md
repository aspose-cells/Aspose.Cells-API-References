---
title: "Workbook.IsLicensed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Anger om licensen är inställd"
type: docs
url: /sv/net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

Anger om licensen är inställd.

```csharp
public bool IsLicensed { get; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsLicensedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Ställ in några grundläggande egenskaper för att demonstrera att arbetsboken används
            wb.Worksheets[0].Name = "Sheet1";
            wb.Worksheets[0].Cells[0, 0].PutValue("Sample Data");
            
            // Kontrollera om arbetsboken är licensierad
            Console.WriteLine($"IsLicensed: {wb.IsLicensed}");
            
            // Demonstrera olika beteenden baserat på licensstatus
            if (wb.IsLicensed)
            {
                Console.WriteLine("Running in licensed mode - full features available");
            }
            else
            {
                Console.WriteLine("Running in evaluation mode - watermarks will appear");
            }

            // Spara till minnesström för att demonstrera funktionaliteten
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                Console.WriteLine($"Workbook saved successfully (Size: {ms.Length} bytes)");
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


