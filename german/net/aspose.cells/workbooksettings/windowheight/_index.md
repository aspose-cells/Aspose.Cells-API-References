---
title: "WorkbookSettings.WindowHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Die Höhe des Fensters in Punkt"
type: docs
url: /de/net/aspose.cells/workbooksettings/windowheight/
---
## WorkbookSettings.WindowHeight property

Die Höhe des Fensters, gemessen in Punkten.

```csharp
public double WindowHeight { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;
            
            // Setze die WindowHeight-Eigenschaft
            settings.WindowHeight = 600;
            
            // Überprüfe den WindowHeight-Wert
            Console.WriteLine("Window Height set to: " + settings.WindowHeight);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WindowHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


