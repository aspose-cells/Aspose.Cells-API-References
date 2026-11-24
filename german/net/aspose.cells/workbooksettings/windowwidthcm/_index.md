---
title: "WorkbookSettings.WindowWidthCM"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings property. Die Breite des Fensters in Zentimetern"
type: docs
url: /de/net/aspose.cells/workbooksettings/windowwidthcm/
---
## WorkbookSettings.WindowWidthCM property

Die Breite des Fensters, in der Einheit Zentimeter.

```csharp
public double WindowWidthCM { get; set; }
```

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthCMDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;
            
            // Set WindowWidthCM property (20,32 cm = ~8 Zoll)
            settings.WindowWidthCM = 20.32;
            
            // Überprüfe die Einstellung, indem du sie ausgibst
            Console.WriteLine("Window Width in Centimeters: " + settings.WindowWidthCM);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WindowWidthCMDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


