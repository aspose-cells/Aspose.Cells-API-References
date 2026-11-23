---
title: "Classe ShapeGuideCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.ShapeGuideCollection. Encapsule une collection de guides de forme"
type: docs
url: /fr/net/aspose.cells.drawing/shapeguidecollection/
---
## ShapeGuideCollection class

Encapsule une collection de guides de forme

```csharp
public class ShapeGuideCollection : CollectionBase<ShapeGuide>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ShapeGuideCollection](shapeguidecollection/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapeguidecollection/item/) { get; } | Obtient un guide de forme par index |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapeguidecollection/add/)(string, double) | Ajoute un guide de forme.(Important : Cette fonctionnalité n'est actuellement disponible que pour Excel07 et versions ultérieures) |
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

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez une forme personnalisée en utilisant un MsoDrawingType valide et définissez son type sur Rectangle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 0, 0, 200, 100);
            shape.AutoShapeType = AutoShapeType.Rectangle;
            
            // Obtenez le ShapeGuideCollection à partir des ajustements géométriques de la forme
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;
            
            // Ajoutez de nouveaux guides de forme avec des noms et des valeurs
            shapeGuides.Add("Guide1", 0.2);
            shapeGuides.Add("Guide2", 0.5);
            shapeGuides.Add("Guide3", 0.8);
            
            // Récupérer et afficher la valeur du premier guide
            ShapeGuide firstGuide = shapeGuides[0];
            Console.WriteLine($"First guide value: {firstGuide.Value}");
            
            // Enregistrez le classeur
            workbook.Save("ShapeGuideCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeGuide](../shapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


