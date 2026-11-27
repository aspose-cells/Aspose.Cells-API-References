---
title: "ShapePath.PathSegementList"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePath-egenskap. Hämtar ShapeSegmentPathCollection-lista"
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/pathsegementlist/
---
## ShapePath.PathSegementList property

Hämtar [`ShapeSegmentPathCollection`](../../shapesegmentpathcollection/) lista

```csharp
[Obsolete("Use ShapePath.PathSegments property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ShapeSegmentPathCollection PathSegementList { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället ShapePath.PathSegments-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyPathSegementListDemo
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

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("ShapePathPropertyPathSegementListDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeSegmentPathCollection](../../shapesegmentpathcollection/)
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


