---
title: "Klass ShapeSegmentPathCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapeSegmentPathCollection-klass. Representerar en skapandeväg bestående av en serie flyttningar, linjer och kurvor som när de kombineras bildar en geometrisk form"
type: docs
url: /sv/net/aspose.cells.drawing/shapesegmentpathcollection/
---
## ShapeSegmentPathCollection class

Representerar en skapandeväg bestående av en serie rörelser, linjer och kurvor som när de kombineras bildar en geometrisk form.

```csharp
public class ShapeSegmentPathCollection : CollectionBase<ShapeSegmentPath>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ShapeSegmentPathCollection](shapesegmentpathcollection/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapesegmentpathcollection/item/) { get; } | Hämtar [`ShapeSegmentPath`](../shapesegmentpath/) objekt. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapesegmentpathcollection/add/)(ShapePathType) | Lägg till en segmentväg i skapandevägen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeSegmentPath) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeSegmentPath, IComparer&lt;ShapeSegmentPath&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ShapeSegmentPath, IComparer&lt;ShapeSegmentPath&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ShapeSegmentPath) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeSegmentPath[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeSegmentPath[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ShapeSegmentPath[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeSegmentPath) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeSegmentPath, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeSegmentPath, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeSegmentPath) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeSegmentPath, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeSegmentPath, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en ShapePath för att arbeta med segment
                ShapePath path = new ShapePath();

                // Starta en ny sökväg
                path.MoveTo(10, 10);

                // Rita ett linjesegment
                path.LineTo(100, 100);

                // Hämta ShapeSegmentPathCollection från vägen
                ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

                // Lägg till ett stängt segment i vägen.
                int index = segmentPaths.Add(ShapePathType.Close);

                // Visa information om samlingen
                Console.WriteLine($"Number of path segments: {segmentPaths.Count}");
                Console.WriteLine($"Added segment at index: {index}");

                // Åtkomst till det första segmentet (skrivskyddad egenskap)
                if (segmentPaths.Count > 0)
                {
                    ShapeSegmentPath firstSegment = segmentPaths[0];
                    Console.WriteLine($"First segment type: {firstSegment.Type}");
                }

                // Lägg till formen i kalkylbladet
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

                // Spara arbetsboken
                workbook.Save("ShapeSegmentPathCollectionDemo.xlsx");
                Console.WriteLine("ShapeSegmentPathCollection demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ShapeSegmentPathCollection demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeSegmentPath](../shapesegmentpath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


