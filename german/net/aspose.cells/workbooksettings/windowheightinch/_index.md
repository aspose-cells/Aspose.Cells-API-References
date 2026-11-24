---
title: "WorkbookSettings.WindowHeightInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Die Höhe des Fensters in Zoll"
type: docs
url: /de/net/aspose.cells/workbooksettings/windowheightinch/
---
## WorkbookSettings.WindowHeightInch property

Die Höhe des Fensters, gemessen in Zoll.

```csharp
public double WindowHeightInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightInchDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Fensterhöhe in Zoll festlegen
            settings.WindowHeightInch = 5.5;

            // Fensterhöhe in Zoll anzeigen
            Console.WriteLine("Window Height in Inches: " + settings.WindowHeightInch);

            // Speichere die Arbeitsmappe
            workbook.Save("WindowHeightInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


