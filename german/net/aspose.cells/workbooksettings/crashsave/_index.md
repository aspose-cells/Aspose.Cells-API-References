---
title: "WorkbookSettings.CrashSave"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob die Anwendung die Arbeitsmappe nach einem Absturz zuletzt gespeichert hat"
type: docs
url: /de/net/aspose.cells/workbooksettings/crashsave/
---
## WorkbookSettings.CrashSave property

Gibt an, ob die Anwendung die Arbeitsmappe nach einem Absturz zuletzt gespeichert hat.

```csharp
public bool CrashSave { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("CrashSave Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Demonstrieren Sie die CrashSave-Eigenschaft
            settings.CrashSave = true;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Speichern mit aktivierter Crash‑Speicherung
            workbook.Save("CrashSaveEnabled.xlsx");

            // Crash‑Speicherung deaktivieren
            settings.CrashSave = false;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Speichern mit deaktivierter Crash‑Speicherung
            workbook.Save("CrashSaveDisabled.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


