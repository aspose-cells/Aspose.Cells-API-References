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
| [Add](../../aspose.cells.drawing/shapepathpointcollection/add/)(int, int) | Adds a path point. |
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
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create and configure the shape path using drawing commands
            ShapePath path = new ShapePath();
            path.MoveTo(0, 0);
            path.LineTo(4000, 0);
            path.LineTo(4000, 1000);
            path.LineTo(2000, 1500);
            path.LineTo(0, 1000);
            path.LineTo(0, 0);
            path.Close();
            
            // Add freeform shape with the configured path
            Shape shape = worksheet.Shapes.AddFreeform( // Corrected method name
                upperLeftRow: 10,
                top: 10,
                upperLeftColumn: 0,
                left: 0,
                height: 2000,
                width: 2000,
                paths: new ShapePath[] { path }
            );
            
            // Access geometry configuration through the shape
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            
            // Demonstrate collection properties
            Console.WriteLine($"Total paths in shape: {geometry?.Paths.Count ?? 0}");
            if (geometry?.Paths.Count > 0)
            {
                Console.WriteLine($"Path segment count: {geometry.Paths[0].PathSegementList.Count}");
            }
            
            // Save the modified workbook
            workbook.Save("ShapePathPointCollectionDemo.xlsx");
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapePathPoint](../shapepathpoint/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


