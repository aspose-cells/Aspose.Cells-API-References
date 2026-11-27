---
title: "Enum DisplayDrawingObjects"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DisplayDrawingObjects enum. Representerar om och hur objekt ska visas i arbetsboken"
type: docs
url: /sv/net/aspose.cells/displaydrawingobjects/
---
## DisplayDrawingObjects enumeration

Representerar om och hur objekt ska visas i arbetsboken.

```csharp
public enum DisplayDrawingObjects
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| DisplayShapes | `0` | Visa alla objekt |
| Placeholders | `1` | Visa platshållare |
| Hide | `2` | Dölj alla former. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DisplayDrawingObjectsDemo
    {
        public static void DisplayDrawingObjectsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt arbetsbokens inställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in egenskapen DisplayDrawingObjects för att visa alla objekt
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;

            // Spara arbetsboken
            workbook.Save("DisplayDrawingObjectsExample_DisplayShapes.xlsx");

            // Ställ in egenskapen DisplayDrawingObjects för att visa platshållare
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;

            // Spara arbetsboken
            workbook.Save("DisplayDrawingObjectsExample_Placeholders.xlsx");

            // Ställ in egenskapen DisplayDrawingObjects för att dölja alla former
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;

            // Spara arbetsboken
            workbook.Save("DisplayDrawingObjectsExample_Hide.xlsx");
            workbook.Save("DisplayDrawingObjectsExample_Hide.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


