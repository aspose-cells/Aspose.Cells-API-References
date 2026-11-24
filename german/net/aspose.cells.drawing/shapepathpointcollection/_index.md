---
title: "Klasse ShapePathPointCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapePathPointCollection-Klasse. Stellt alle Formpfadpunkte dar"
type: docs
url: /de/net/aspose.cells.drawing/shapepathpointcollection/
---
## ShapePathPointCollection class

Stellt alle Pfadpunkte der Form dar.

```csharp
public class ShapePathPointCollection : CollectionBase<ShapePathPoint>
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ShapePathPointCollection](shapepathpointcollection/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapepathpointcollection/item/) { get; } | Liefert den Formpfadpunkt nach Index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapepathpointcollection/add/)(int, int) | (**Obsolete.**) Fügt einen Pfadpunkt in EMU-Einheiten hinzu. |
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

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstellen Sie eine Instanz der ShapePathPointCollection-Klasse
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Fügen Sie Punkte zur Sammlung mit der Add-Methode hinzu
                pathPoints.Add(10, 10);
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Greifen Sie über die Item-Eigenschaft (Indexer) auf Punkte zu
                Console.WriteLine("Shape path points:");
                for (int i = 0; i < pathPoints.Count; i++)
                {
                    ShapePathPoint point = pathPoints[i];
                    Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
                }

                // Erstellen Sie einen Formpfad und verwenden Sie die Punkte
                ShapePath path = new ShapePath();
                path.MoveTo(10, 10);
                foreach (ShapePathPoint point in pathPoints)
                {
                    path.LineTo(point.X, point.Y);
                }
                path.Close();

                // Eine Freiformform zum Arbeitsblatt hinzufügen
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapePathPoint](../shapepathpoint/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


