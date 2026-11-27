---
title: "WorkbookSettings.AutoRecover"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Anger om filen är markerad för automatisk återställning"
type: docs
url: /sv/net/aspose.cells/workbooksettings/autorecover/
---
## WorkbookSettings.AutoRecover property

Anger om filen är markerad för automatisk återställning.

```csharp
public bool AutoRecover { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoRecoverDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in AutoRecover och andra inställningar
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Spara arbetsboken
            string outputPath = "WorkbookSettings_AutoRecoverDemo.xlsx";
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


