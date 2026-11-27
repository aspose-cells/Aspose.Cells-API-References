---
title: "WorkbookSettings.IsMinimized"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Representerar om det genererade kalkylbladet kommer att öppnas minimerat"
type: docs
url: /sv/net/aspose.cells/workbooksettings/isminimized/
---
## WorkbookSettings.IsMinimized property

Anger om det genererade kalkylbladet kommer att öppnas minimerat.

```csharp
public bool IsMinimized { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsMinimizedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in IsMinimized-egenskapen till true
            workbook.Settings.IsMinimized = true;

            // Spara arbetsboken
            workbook.Save("IsMinimizedDemo.xlsx");

            // Läs in den sparade arbetsboken för att verifiera egenskapen
            Workbook loadedWorkbook = new Workbook("IsMinimizedDemo.xlsx");

            // Skriv ut värdet för IsMinimized-egenskapen
            Console.WriteLine("Workbook IsMinimized property: " + loadedWorkbook.Settings.IsMinimized);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


