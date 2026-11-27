---
title: "ShapeCollection.AddIcons"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till svg-bild"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection.AddIcons method

Lägger till en svg-bild.

```csharp
public Picture AddIcons(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageByteData, byte[] compatibleImageData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för formen från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Det horisontella offsetet för formen från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Höjden på formen, i enhet pixel. |
| bredd | Int32 | Bredden på formen, i enhet pixel. |
| imageByteData | Byte[] | Bildens byte-data. |
| compatibleImageData | Byte[] | Konverterad bilddata från svg för att vara kompatibel med Excel 2016 eller lägre versioner. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddIconsWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Skapa en exempelikonfil (vid verklig användning skulle du använda en befintlig fil)
            string iconPath = "icon.svg";
            File.WriteAllText(iconPath, "<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><circle cx='50' cy='50' r='40' fill='red'/></svg>");

            // Lägg till ikon i kalkylbladet
            using (FileStream fs = new FileStream(iconPath, FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Rensa upp (valfritt)
            File.Delete(iconPath);
        }
    }
}
```

### Se även

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


