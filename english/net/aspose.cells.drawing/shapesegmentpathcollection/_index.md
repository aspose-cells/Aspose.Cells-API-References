---
title: Class ShapeSegmentPathCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ShapeSegmentPathCollection class. Represents a creation path consisting of a series of moves lines and curves that when combined will form a geometric shape
type: docs
url: /net/aspose.cells.drawing/shapesegmentpathcollection/
---
## ShapeSegmentPathCollection class

Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.

```csharp
public class ShapeSegmentPathCollection : CollectionBase<ShapeSegmentPath>
```

## Constructors

| Name | Description |
| --- | --- |
| [ShapeSegmentPathCollection](shapesegmentpathcollection/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapesegmentpathcollection/item/) { get; } | Gets [`ShapeSegmentPath`](../shapesegmentpath/) object. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapesegmentpathcollection/add/)(ShapePathType) | Add a segment path in creation path. |
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

### Examples

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
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a ShapePath to work with segments
                ShapePath path = new ShapePath();

                // Start a new path
                path.MoveTo(10, 10);

                // Draw a line segment
                path.LineTo(100, 100);

                // Get the ShapeSegmentPathCollection from the path
                ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

                // Add a close path segment
                int index = segmentPaths.Add(ShapePathType.Close);

                // Display information about the collection
                Console.WriteLine($"Number of path segments: {segmentPaths.Count}");
                Console.WriteLine($"Added segment at index: {index}");

                // Access the first segment (read-only property)
                if (segmentPaths.Count > 0)
                {
                    ShapeSegmentPath firstSegment = segmentPaths[0];
                    Console.WriteLine($"First segment type: {firstSegment.Type}");
                }

                // Add the shape to the worksheet
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

                // Save the workbook
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

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeSegmentPath](../shapesegmentpath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


