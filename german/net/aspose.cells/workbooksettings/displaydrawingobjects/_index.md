---
title: "WorkbookSettings.DisplayDrawingObjects"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob und wie Objekte im Arbeitsbuch angezeigt werden"
type: docs
url: /de/net/aspose.cells/workbooksettings/displaydrawingobjects/
---
## WorkbookSettings.DisplayDrawingObjects property

Gibt an, ob und wie Objekte im Workbook angezeigt werden.

```csharp
public DisplayDrawingObjects DisplayDrawingObjects { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDisplayDrawingObjectsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf die Arbeitsmappeneinstellungen zu
            WorkbookSettings settings = workbook.Settings;

            // Füge eine Beispielform hinzu, um die Eigenschaft zu demonstrieren
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Setze auf Anzeige aller Formen
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
            workbook.Save("DisplayShapes.xlsx");

            // Setze auf Anzeige von Platzhaltern
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;
            workbook.Save("Placeholders.xlsx");

            // Setze auf Ausblenden aller Formen
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;
            workbook.Save("Hide.xlsx");
        }
    }
}
```

### Siehe auch

* enum [DisplayDrawingObjects](../../displaydrawingobjects/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


