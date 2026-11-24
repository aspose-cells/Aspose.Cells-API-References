---
title: "WorkbookSettings.WindowLeft"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings property. Der Abstand vom linken Rand des Clientbereichs bis zum linken Rand des Fensters in Punkt"
type: docs
url: /de/net/aspose.cells/workbooksettings/windowleft/
---
## WorkbookSettings.WindowLeft property

Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters, gemessen in Punkten.

```csharp
public double WindowLeft { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;

            // Set WindowLeft property, um das Fenster 100 Pixel vom linken Rand zu positionieren
            settings.WindowLeft = 100;

            // Setze weitere Fenstereigenschaften zur Demonstration
            settings.WindowTop = 50;
            settings.WindowWidth = 800;
            settings.WindowHeight = 600;

            // Beispieldaten zum Arbeitsblatt hinzufügen
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Left: {settings.WindowLeft}px");
            sheet.Cells["A3"].PutValue($"Top: {settings.WindowTop}px");

            // Speichere die Arbeitsmappe
            workbook.Save("WindowPositionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


