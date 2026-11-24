---
title: "WorkbookSettings.WindowLeftInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters. In Zoll"
type: docs
url: /de/net/aspose.cells/workbooksettings/windowleftinch/
---
## WorkbookSettings.WindowLeftInch property

Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters, gemessen in Zoll.

```csharp
public double WindowLeftInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftInchDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;

            // Setze die WindowLeftInch-Eigenschaft
            settings.WindowLeftInch = 1.5; // Position window 1.5 inches from left edge of screen

            // Füge einige Beispieldaten hinzu, um zu demonstrieren, dass die Arbeitsmappe funktional ist
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Window left position: {settings.WindowLeftInch} inches");

            // Speichere die Arbeitsmappe
            workbook.Save("WindowLeftInchDemo.xlsx");

            Console.WriteLine("Workbook saved with WindowLeftInch = " + settings.WindowLeftInch);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


