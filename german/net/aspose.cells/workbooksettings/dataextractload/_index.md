---
title: "WorkbookSettings.DataExtractLoad"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob die Anwendung die Arbeitsmappe zuletzt zur Datenwiederherstellung geöffnet hat"
type: docs
url: /de/net/aspose.cells/workbooksettings/dataextractload/
---
## WorkbookSettings.DataExtractLoad property

Gibt an, ob die Anwendung die Arbeitsmappe zuletzt zur Datenwiederherstellung geöffnet hat.

```csharp
public bool DataExtractLoad { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDataExtractLoadDemo
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
            string destPath = "output.xlsx";
            workbook.Save(destPath);
            
            // Arbeitsmappe neu laden, um die Einstellungen zu überprüfen
            Workbook loadedWorkbook = new Workbook(destPath);
            
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


