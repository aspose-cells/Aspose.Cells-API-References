---
title: "Klasse ShapeGuideCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapeGuideCollection Klasse. Kapselt eine Sammlung von Shape Guides"
type: docs
url: /de/net/aspose.cells.drawing/shapeguidecollection/
---
## ShapeGuideCollection class

Kapselt eine Sammlung von Shape-Guides

```csharp
public class ShapeGuideCollection : CollectionBase<ShapeGuide>
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ShapeGuideCollection](shapeguidecollection/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapeguidecollection/item/) { get; } | Ruft einen Shape Guide nach Index ab |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapeguidecollection/add/)(string, double) | Fügt einen Shape Guide hinzu. (Wichtig: Diese Funktion ist derzeit nur für Excel07 und höher verfügbar) |
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

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie eine benutzerdefinierte Form mit gültigem MsoDrawingType hinzu und setzen Sie deren Typ auf Rectangle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 0, 0, 200, 100);
            shape.AutoShapeType = AutoShapeType.Rectangle;
            
            // Holen Sie die ShapeGuideCollection aus den Geometrieanpassungen der Form
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;
            
            // Fügen Sie neue Shape Guides mit Namen und Werten hinzu
            shapeGuides.Add("Guide1", 0.2);
            shapeGuides.Add("Guide2", 0.5);
            shapeGuides.Add("Guide3", 0.8);
            
            // Rufen Sie den Wert des ersten Guides ab und zeigen Sie ihn an
            ShapeGuide firstGuide = shapeGuides[0];
            Console.WriteLine($"First guide value: {firstGuide.Value}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShapeGuideCollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeGuide](../shapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


