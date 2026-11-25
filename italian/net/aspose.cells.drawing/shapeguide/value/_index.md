---
title: "ShapeGuide.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeGuide. Ottiene o imposta il valore di questa guida"
type: docs
url: /it/net/aspose.cells.drawing/shapeguide/value/
---
## ShapeGuide.Value property

Ottiene o imposta il valore di questa guida

```csharp
public double Value { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuidePropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma che utilizza guide di regolazione
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


            Console.WriteLine("Updated adjustment values");

            shapeGuides[0].Value = 25.5;
            shapeGuides[1].Value = 25.5;
            shapeGuides[2].Value = 25.5;
            shapeGuides[3].Value = 25.5;            

            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);
            
            // Salva la cartella di lavoro modificata
            workbook.Save("ShapeGuideValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeGuide](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


