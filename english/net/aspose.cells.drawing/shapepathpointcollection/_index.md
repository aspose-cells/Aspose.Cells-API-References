---
title: Class ShapePathPointCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ShapePathPointCollection class. Represents all shape path points
type: docs
url: /net/aspose.cells.drawing/shapepathpointcollection/
---
## ShapePathPointCollection class

Represents all shape path points.

```csharp
public class ShapePathPointCollection : CollectionBase<ShapePathPoint>
```

## Constructors

| Name | Description |
| --- | --- |
| [ShapePathPointCollection](shapepathpointcollection/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapepathpointcollection/item/) { get; } | Gets shape path point by index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapepathpointcollection/add/)(int, int) | (**Obsolete.**) Adds a path point in unit of EMUs. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapePathPoint) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapePathPoint, IComparer&lt;ShapePathPoint&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ShapePathPoint, IComparer&lt;ShapePathPoint&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ShapePathPoint) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapePathPoint[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapePathPoint[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ShapePathPoint[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ShapePathPoint&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ShapePathPoint&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ShapePathPoint&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ShapePathPoint&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ShapePathPoint&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ShapePathPoint&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ShapePathPoint&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ShapePathPoint&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ShapePathPoint&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ShapePathPoint&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapePathPoint) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapePathPoint, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapePathPoint, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapePathPoint) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapePathPoint, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapePathPoint, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointCollectionDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create an instance of the ShapePathPointCollection class
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Add points to the collection using the Add method
                pathPoints.Add(10, 10);
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Access points using the Item property (indexer)
                Console.WriteLine("Shape path points:");
                for (int i = 0; i < pathPoints.Count; i++)
                {
                    ShapePathPoint point = pathPoints[i];
                    Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
                }

                // Create a shape path and use the points
                ShapePath path = new ShapePath();
                path.MoveTo(10, 10);
                foreach (ShapePathPoint point in pathPoints)
                {
                    path.LineTo(point.X, point.Y);
                }
                path.Close();

                // Add a freeform shape to the worksheet
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Save the workbook
                workbook.Save("ShapePathPointCollectionDemo.xlsx");
                Console.WriteLine("ShapePathPointCollection demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPointCollection: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapePathPoint](../shapepathpoint/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


