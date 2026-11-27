---
title: "WorkbookSettings.CheckCustomNumberFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Anger om kontroll av anpassat talformat ska göras när Style.Custom sätts"
type: docs
url: /sv/net/aspose.cells/workbooksettings/checkcustomnumberformat/
---
## WorkbookSettings.CheckCustomNumberFormat property

Anger om anpassat talformat ska kontrolleras när Style.Custom sätts.

```csharp
public bool CheckCustomNumberFormat { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCustomNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            
            // Ställ först in ett giltigt anpassat talformat
            style.Custom = "#,##0.00";
            
            // Aktivera strikt kontroll
            workbook.Settings.CheckCustomNumberFormat = true;
            
            try
            {
                // Försök att sätta ett ogiltigt anpassat talformat
                style.Custom = "fff @ ggg";
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error setting custom format: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


