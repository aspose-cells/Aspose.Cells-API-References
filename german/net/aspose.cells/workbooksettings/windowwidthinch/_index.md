---
title: "WorkbookSettings.WindowWidthInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Die Breite des Fensters in Zoll."
type: docs
url: /de/net/aspose.cells/workbooksettings/windowwidthinch/
---
## WorkbookSettings.WindowWidthInch property

Die Breite des Fensters, in der Einheit Zoll.

```csharp
public double WindowWidthInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthInchDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Fensterbreite in Zoll festlegen
            settings.WindowWidthInch = 10.5;

            // Fensterbreite in Zoll anzeigen
            Console.WriteLine("Window Width in Inches: " + settings.WindowWidthInch);

            // Speichere die Arbeitsmappe
            workbook.Save("WindowWidthInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


