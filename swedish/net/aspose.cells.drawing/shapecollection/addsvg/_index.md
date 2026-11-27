---
title: "ShapeCollection.AddSvg"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till svg-bild"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addsvg/
---
## ShapeCollection.AddSvg method

Lägger till en svg-bild.

```csharp
public Picture AddSvg(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] svgData, byte[] compatibleImageData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för formen från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Det horisontella offsetet för formen från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Höjden på formen, i enhet pixel. |
| bredd | Int32 | Bredden på formen, i enhet pixel. |
| svgData | Byte[] | Svg-bilddata. |
| compatibleImageData | Byte[] | Konverterad bilddata från svg för att vara kompatibel med Excel 2016 eller lägre versioner. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSvgWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.ShapeCollection shapes = worksheet.Shapes;

            // Läs in SVG-fil
            using (FileStream fs = new FileStream("image.svg", FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                
                // Lägg till SVG i kalkylbladet
                Aspose.Cells.Drawing.Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


