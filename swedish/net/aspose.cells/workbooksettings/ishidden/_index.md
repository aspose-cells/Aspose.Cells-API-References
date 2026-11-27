---
title: "WorkbookSettings.IsHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Anger om denna arbetsbok är dold"
type: docs
url: /sv/net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

Anger om denna arbetsbok är dold.

```csharp
public bool IsHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in IsHidden-egenskapen till true
            settings.IsHidden = true;
            Console.WriteLine("Workbook is hidden: " + settings.IsHidden);

            // Spara arbetsboken
            workbook.Save("WorkbookSettings_IsHidden_True.xlsx");

            // Skapa en annan arbetsbok
            Workbook workbook2 = new Workbook();

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings2 = workbook2.Settings;

            // Ställ in IsHidden-egenskapen till false (standard)
            settings2.IsHidden = false;
            Console.WriteLine("Workbook is hidden: " + settings2.IsHidden);

            // Spara arbetsboken
            workbook2.Save("WorkbookSettings_IsHidden_False.xlsx");

            // Läs in och kontrollera de sparade arbetsböckerna
            Workbook loadedWorkbook1 = new Workbook("WorkbookSettings_IsHidden_True.xlsx");
            Console.WriteLine("Loaded workbook1 is hidden: " + loadedWorkbook1.Settings.IsHidden);

            Workbook loadedWorkbook2 = new Workbook("WorkbookSettings_IsHidden_False.xlsx");
            Console.WriteLine("Loaded workbook2 is hidden: " + loadedWorkbook2.Settings.IsHidden);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


