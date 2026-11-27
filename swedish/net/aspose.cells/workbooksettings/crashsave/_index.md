---
title: "WorkbookSettings.CrashSave"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Anger om applikationen senast sparade arbetsboksfilen efter en krasch"
type: docs
url: /sv/net/aspose.cells/workbooksettings/crashsave/
---
## WorkbookSettings.CrashSave property

Anger om programmet senast sparade arbetsboksfilen efter en krasch.

```csharp
public bool CrashSave { get; set; }
```

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCrashSaveDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("CrashSave Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Demonstrera CrashSave-egenskapen
            settings.CrashSave = true;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Spara med kraschlagring aktiverad
            workbook.Save("CrashSaveEnabled.xlsx");

            // Inaktivera kraschlagring
            settings.CrashSave = false;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Spara med kraschlagring inaktiverad
            workbook.Save("CrashSaveDisabled.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


