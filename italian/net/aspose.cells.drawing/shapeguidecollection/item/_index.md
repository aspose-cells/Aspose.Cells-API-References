---
title: "ShapeGuideCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeGuideCollection. Ottiene una guida di forma per indice"
type: docs
url: /it/net/aspose.cells.drawing/shapeguidecollection/item/
---
## ShapeGuideCollection indexer

Ottiene una guida di forma per indice

```csharp
public ShapeGuide this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma che utilizza guide di regolazione
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            // Accedi alla collezione di guide di regolazione della forma tramite Geometry
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

            // Aggiungi nuove guide alla collezione
            shapeGuides.Add("adj1", 25.5);
            shapeGuides.Add("adj2", 30);
            shapeGuides.Add("adj3", 25.5);
            shapeGuides.Add("adj4", 35);

            // Dimostra la lettura dei valori delle guide (proprietà Name non disponibile nella definizione fornita)
            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);

            // Salva la cartella di lavoro modificata
            workbook.Save("ShapeGuideCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeGuide](../../shapeguide/)
* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


