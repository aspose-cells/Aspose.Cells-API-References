---
title: "WorkbookSettings.MemorySetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt die Optionen zur Speicherverwendung zurück oder legt sie fest. Die neue Option wird als Standardoption für neu erstellte Arbeitsblätter übernommen, wirkt sich jedoch nicht auf bereits vorhandene Arbeitsblätter aus."
type: docs
url: /de/net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

Liest oder setzt die Speicherverbrauchsoptionen. Die neue Option wird als Standardoption für neu erstellte Arbeitsblätter übernommen, wirkt jedoch nicht für bestehende Arbeitsblätter.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Hinweise

Weitere Details zum Speichermodus finden Sie unter [`MemorySetting`](../../cells/memorysetting/).

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit der Speicherpräferenz-Einstellung
            Workbook wb = new Workbook();
            wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Daten hinzu
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Memory Setting Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // In einen Memory-Stream im PDF-Format speichern
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Pdf);
                Console.WriteLine("Workbook saved to PDF with MemoryPreference setting");
            }
        }
    }
}
```

### Siehe auch

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


