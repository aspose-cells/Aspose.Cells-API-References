##Class ShapeGuideCollection
Aspose.Cells.Drawing.ShapeGuideCollection class. Encapsulates a collection of shape guide
## ShapeGuideCollection class
Encapsulates a collection of shape guide
```csharp
public class ShapeGuideCollection : CollectionBase<ShapeGuide>
```
## Constructors
| Name | Description |
| --- | --- |
| [ShapeGuideCollection](shapeguidecollection/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapeguidecollection/item/) { get; } | Gets a shape guide by index |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapeguidecollection/add/)(string, double) | Adds a shape guide.(Important: This feature is currently only available for Excel07 and above) |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeGuide) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeGuide, IComparer&lt;ShapeGuide&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ShapeGuide, IComparer&lt;ShapeGuide&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ShapeGuide) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeGuide[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeGuide[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ShapeGuide[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ShapeGuide&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ShapeGuide&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ShapeGuide&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ShapeGuide&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ShapeGuide&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeGuide) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeGuide, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeGuide, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeGuide) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeGuide, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeGuide, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassShapeGuideCollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a custom shape using valid MsoDrawingType and set its type to Rectangle
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 0, 0, 200, 100);
shape.AutoShapeType = AutoShapeType.Rectangle;
// Get the ShapeGuideCollection from the shape's geometry adjustments
ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;
// Add new shape guides with names and values
shapeGuides.Add("Guide1", 0.2);
shapeGuides.Add("Guide2", 0.5);
shapeGuides.Add("Guide3", 0.8);
// Retrieve and display the first guide's value
ShapeGuide firstGuide = shapeGuides[0];
Console.WriteLine($"First guide value: {firstGuide.Value}");
// Save the workbook
workbook.Save("ShapeGuideCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeGuide](../shapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
