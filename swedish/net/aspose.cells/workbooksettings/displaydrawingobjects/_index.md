---
title: "WorkbookSettings.DisplayDrawingObjects"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Anger om och hur objekt ska visas i arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbooksettings/displaydrawingobjects/
---
## WorkbookSettings.DisplayDrawingObjects property

Anger om och hur objekt ska visas i arbetsboken.

```csharp
public DisplayDrawingObjects DisplayDrawingObjects { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDisplayDrawingObjectsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt arbetsbokens inställningar
            WorkbookSettings settings = workbook.Settings;

            // Lägg till en exempelform för att demonstrera egenskapen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ställ in att visa alla former
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
            workbook.Save("DisplayShapes.xlsx");

            // Ställ in att visa platshållare
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;
            workbook.Save("Placeholders.xlsx");

            // Ställ in att dölja alla former
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;
            workbook.Save("Hide.xlsx");
        }
    }
}
```

### Se även

* enum [DisplayDrawingObjects](../../displaydrawingobjects/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


