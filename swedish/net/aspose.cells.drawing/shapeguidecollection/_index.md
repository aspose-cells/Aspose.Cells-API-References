---
title: "Klass ShapeGuideCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapeGuideCollection-klass. Inkapslar en samling av formguider"
type: docs
url: /sv/net/aspose.cells.drawing/shapeguidecollection/
---
## ShapeGuideCollection class

Inkapslar en samling av formguider

```csharp
public class ShapeGuideCollection : CollectionBase<ShapeGuide>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ShapeGuideCollection](shapeguidecollection/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapeguidecollection/item/) { get; } | Hämtar en formguide efter index |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapeguidecollection/add/)(string, double) | Lägger till en formguide. (Viktigt: Denna funktion är för närvarande endast tillgänglig för Excel07 och senare) |
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

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en anpassad form med giltig MsoDrawingType och sätt dess typ till Rectangle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 0, 0, 200, 100);
            shape.AutoShapeType = AutoShapeType.Rectangle;
            
            // Hämta ShapeGuideCollection från formens geometrijusteringar
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;
            
            // Lägg till nya formguider med namn och värden
            shapeGuides.Add("Guide1", 0.2);
            shapeGuides.Add("Guide2", 0.5);
            shapeGuides.Add("Guide3", 0.8);
            
            // Hämta och visa det första guidens värde
            ShapeGuide firstGuide = shapeGuides[0];
            Console.WriteLine($"First guide value: {firstGuide.Value}");
            
            // Spara arbetsboken
            workbook.Save("ShapeGuideCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeGuide](../shapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


