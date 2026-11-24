---
title: "WorkbookSettings.CheckCustomNumberFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob beim Festlegen von Style.Custom die benutzerdefinierte Zahlenformatprüfung durchgeführt wird"
type: docs
url: /de/net/aspose.cells/workbooksettings/checkcustomnumberformat/
---
## WorkbookSettings.CheckCustomNumberFormat property

Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat geprüft wird.

```csharp
public bool CheckCustomNumberFormat { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCustomNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            
            // Zuerst ein gültiges benutzerdefiniertes Zahlenformat festlegen
            style.Custom = "#,##0.00";
            
            // Strenge Prüfung aktivieren
            workbook.Settings.CheckCustomNumberFormat = true;
            
            try
            {
                // Versuch, ein ungültiges benutzerdefiniertes Zahlenformat festzulegen
                style.Custom = "fff @ ggg";
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error setting custom format: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


