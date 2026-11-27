---
title: "ShapeCollection.AddSpinner"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en Spinner i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

Lägger till en spinner i kalkylbladet.

```csharp
public Spinner AddSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar den vertikala förskjutningen av Spinner från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av Spinner från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar höjden på Spinner, i enhet pixel. |
| bredd | Int32 | Representerar bredden på Spinner, i enhet pixel. |

### Returvärde

Ett Spinner-objekt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en spinner i kalkylbladet
            Aspose.Cells.Drawing.Spinner spinner = (Aspose.Cells.Drawing.Spinner)worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 50);

            // Ange spinner-egenskaper
            spinner.LinkedCell = "A1";
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 1;

            // Spara arbetsboken
            workbook.Save("AddSpinnerDemo.xlsx");
        }
    }
}
```

### Se även

* class [Spinner](../../spinner/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


