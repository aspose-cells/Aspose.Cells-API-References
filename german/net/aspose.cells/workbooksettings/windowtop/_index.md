---
title: "WorkbookSettings.WindowTop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters in Punkt."
type: docs
url: /de/net/aspose.cells/workbooksettings/windowtop/
---
## WorkbookSettings.WindowTop property

Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Punkt.

```csharp
public double WindowTop { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;

            // Setzen Sie die WindowTop-Eigenschaft, um das Fenster 100 Pixel vom oberen Rand zu positionieren.
            settings.WindowTop = 100;
            
            // Überprüfen Sie den WindowTop-Wert.
            Console.WriteLine("Window top position set to: " + settings.WindowTop);

            // Speichere die Arbeitsmappe
            workbook.Save("WindowTopDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


