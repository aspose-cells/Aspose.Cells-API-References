---
title: "WorkbookSettings.RepairLoad"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Anger om applikationen senast öppnade arbetsboken i säkert eller reparationsläge"
type: docs
url: /sv/net/aspose.cells/workbooksettings/repairload/
---
## WorkbookSettings.RepairLoad property

Indikerar om programmet senast öppnade arbetsboken i säkert eller reparationsläge.

```csharp
public bool RepairLoad { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRepairLoadDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Konfigurera arbetsboksinställningar
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Spara arbetsboken
            string outputPath = "WorkbookSettings_RepairLoad_Example.xlsx";
            workbook.Save(outputPath);

            // Läs in den sparade arbetsboken för att verifiera inställningarna
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Skriv ut inställningarna till konsolen
            Console.WriteLine("AutoRecover: " + loadedWorkbook.Settings.AutoRecover);
            Console.WriteLine("DataExtractLoad: " + loadedWorkbook.Settings.DataExtractLoad);
            Console.WriteLine("CrashSave: " + loadedWorkbook.Settings.CrashSave);
            Console.WriteLine("RepairLoad: " + loadedWorkbook.Settings.RepairLoad);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


