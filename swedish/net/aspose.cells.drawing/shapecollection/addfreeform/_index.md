---
title: "ShapeCollection.AddFreeform"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en frihandsform till kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

Lägger till en freeform shape i kalkylbladet.

```csharp
public Shape AddFreeform(int topRow, int top, int leftColumn, int left, int height, int width, 
    ShapePath[] paths)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för frihandsformen från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar det horisontella offsetet för frihandsformen från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar frihandsformens höjd, i enhet pixel. |
| bredd | Int32 | Representerar frihandsformens bredd, i enhet pixel. |
| sökvägar | ShapePath[] | Representerar en användardefinierad sökväg |

### Returvärde

En frihandsform.

### Anmärkningar

Obs: Bredden och höjden i parametrarna kan vara valfria positiva heltalsvärden, inte den totala bredden och höjden för ShapePath‑arrayen som anges av ’paths'. Förhållandet mellan dem är ett skala‑fyll‑förhållande, det vill säga att varje ShapePath‑objekt skalas enligt bredden och höjden. Därför, när det finns flera objekt i 'paths', måste varje ShapePath‑objekt utformas på ett rimligt sätt för att uppfylla förväntningarna. När det bara finns ett ShapePath‑objekt och inga andra krav, är det en bra lösning att skicka objektets bredd och höjd som parametervärden.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeformWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Skapa anpassade figurvägar
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                                96.5f, -7.148871f,
                                130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                                182.24997f, 75.351f,
                                201, 120.517795f);
            shapePath1.MoveTo(150, 80);
            shapePath1.ArcTo(25, 25, 0, 270);
            
            // Lägg till frihandsform i kalkylbladet
            shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1 });

            // Spara arbetsboken
            workbook.Save("AddFreeformDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


