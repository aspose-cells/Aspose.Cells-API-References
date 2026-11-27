---
title: "WorkbookSettings.DataExtractLoad"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. anger om programmet senast öppnade arbetsboken för dataräddning"
type: docs
url: /sv/net/aspose.cells/workbooksettings/dataextractload/
---
## WorkbookSettings.DataExtractLoad property

Anger om programmet senast öppnade arbetsboken för dataräddning.

```csharp
public bool DataExtractLoad { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDataExtractLoadDemo
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
            string destPath = "output.xlsx";
            workbook.Save(destPath);
            
            // Läs in arbetsboken på nytt för att verifiera inställningarna
            Workbook loadedWorkbook = new Workbook(destPath);
            
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


