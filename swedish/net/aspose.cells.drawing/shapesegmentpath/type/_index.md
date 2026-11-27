---
title: "ShapeSegmentPath.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeSegmentPath egenskap. Hämtar segmenttyp för banan"
type: docs
url: /sv/net/aspose.cells.drawing/shapesegmentpath/type/
---
## ShapeSegmentPath.Type property

Hämtar typen av vägsegmentet

```csharp
public ShapePathType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Skapa en ny formbana
                ShapePath shapePath = new ShapePath();

                // Flytta till startpunkten
                shapePath.MoveTo(10, 10);

                // Anropa LineTo metod med (Single, Single) parametrar
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                // Åtkomst till PathSegementList egenskap
                ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;

                // Visa antalet segment i banan
                Console.WriteLine("Number of path segments: " + segmentList.Count);

                // Iterera genom varje segment och visa dess typ
                foreach (ShapeSegmentPath segment in segmentList)
                {
                    Console.WriteLine("Segment type: " + segment.Type);
                }

                //lägg till fri form
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }


            // Spara arbetsboken
            workbook.Save("ShapeSegmentPathTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


