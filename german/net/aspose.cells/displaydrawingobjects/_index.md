---
title: "Aufzählung DisplayDrawingObjects"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DisplayDrawingObjects Aufzählung. Gibt an, ob und wie Objekte in der Arbeitsmappe angezeigt werden."
type: docs
url: /de/net/aspose.cells/displaydrawingobjects/
---
## DisplayDrawingObjects enumeration

Stellt dar, ob und wie Objekte in der Arbeitsmappe angezeigt werden.

```csharp
public enum DisplayDrawingObjects
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DisplayShapes | `0` | Alle Objekte anzeigen |
| Placeholders | `1` | Platzhalter anzeigen |
| Hide | `2` | Alle Formen ausblenden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DisplayDrawingObjectsDemo
    {
        public static void DisplayDrawingObjectsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf die Arbeitsmappeneinstellungen zu
            WorkbookSettings settings = workbook.Settings;

            // Setze die DisplayDrawingObjects-Eigenschaft, um alle Objekte anzuzeigen
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;

            // Speichere die Arbeitsmappe
            workbook.Save("DisplayDrawingObjectsExample_DisplayShapes.xlsx");

            // Setze die DisplayDrawingObjects-Eigenschaft, um Platzhalter anzuzeigen
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;

            // Speichere die Arbeitsmappe
            workbook.Save("DisplayDrawingObjectsExample_Placeholders.xlsx");

            // Setze die DisplayDrawingObjects-Eigenschaft, um alle Formen auszublenden
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;

            // Speichere die Arbeitsmappe
            workbook.Save("DisplayDrawingObjectsExample_Hide.xlsx");
            workbook.Save("DisplayDrawingObjectsExample_Hide.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


