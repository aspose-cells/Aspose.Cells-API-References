---
title: "WorkbookSettings.WindowWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Die Breite des Fensters in Punkt."
type: docs
url: /de/net/aspose.cells/workbooksettings/windowwidth/
---
## WorkbookSettings.WindowWidth property

Die Breite des Fensters, in der Einheit Punkt.

```csharp
public double WindowWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;
            
            // WindowWidth-Eigenschaft festlegen
            settings.WindowWidth = 800;
            
            // Überprüfen Sie den WindowWidth-Wert
            Console.WriteLine("Window Width set to: " + settings.WindowWidth);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WindowWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


