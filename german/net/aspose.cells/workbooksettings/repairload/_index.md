---
title: "WorkbookSettings.RepairLoad"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im sicheren oder Reparaturmodus geöffnet hat"
type: docs
url: /de/net/aspose.cells/workbooksettings/repairload/
---
## WorkbookSettings.RepairLoad property

Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im sicheren oder Reparaturmodus geöffnet hat.

```csharp
public bool RepairLoad { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRepairLoadDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsmappeneinstellungen konfigurieren
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Speichere die Arbeitsmappe
            string outputPath = "WorkbookSettings_RepairLoad_Example.xlsx";
            workbook.Save(outputPath);

            // Laden Sie die gespeicherte Arbeitsmappe, um die Einstellungen zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Einstellungen in die Konsole ausgeben
            Console.WriteLine("AutoRecover: " + loadedWorkbook.Settings.AutoRecover);
            Console.WriteLine("DataExtractLoad: " + loadedWorkbook.Settings.DataExtractLoad);
            Console.WriteLine("CrashSave: " + loadedWorkbook.Settings.CrashSave);
            Console.WriteLine("RepairLoad: " + loadedWorkbook.Settings.RepairLoad);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


