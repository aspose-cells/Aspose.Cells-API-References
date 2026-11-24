---
title: "WorkbookSettings.WindowHeightCM"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings property. Die Höhe des Fensters in Zentimetern"
type: docs
url: /de/net/aspose.cells/workbooksettings/windowheightcm/
---
## WorkbookSettings.WindowHeightCM property

Die Höhe des Fensters, gemessen in Zentimetern.

```csharp
public double WindowHeightCM { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightCMDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Setze WindowHeightCM property
            settings.WindowHeightCM = 15.5;

            // Zeige den gesetzten Wert an
            Console.WriteLine("Window Height in Centimeters: " + settings.WindowHeightCM);

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


