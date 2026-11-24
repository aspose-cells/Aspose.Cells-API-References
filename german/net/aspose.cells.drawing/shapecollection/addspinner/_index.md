---
title: "ShapeCollection.AddSpinner"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt einen Spinner zum Arbeitsblatt hinzu."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

Fügt einen Spinner zum Arbeitsblatt hinzu.

```csharp
public Spinner AddSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz des Spinners von seiner linken Zeile in Pixeln dar. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz des Spinners von seiner linken Spalte in Pixeln dar. |
| Höhe | Int32 | Stellt die Höhe des Spinners in Pixeln dar. |
| Breite | Int32 | Stellt die Breite des Spinners in Pixeln dar. |

### Rückgabewert

Ein Spinner-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSpinnerWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einen Spinner zum Arbeitsblatt hinzu
            Aspose.Cells.Drawing.Spinner spinner = (Aspose.Cells.Drawing.Spinner)worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 50);

            // Spinner-Eigenschaften festlegen
            spinner.LinkedCell = "A1";
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 1;

            // Speichere die Arbeitsmappe
            workbook.Save("AddSpinnerDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Spinner](../../spinner/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


