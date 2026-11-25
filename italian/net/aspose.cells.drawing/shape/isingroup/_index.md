---
title: "Shape.IsInGroup"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se la forma è raggruppata"
type: docs
url: /it/net/aspose.cells.drawing/shape/isingroup/
---
## Shape.IsInGroup property

Indica se la shape è raggruppata.

```csharp
public bool IsInGroup { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyIsInGroupDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcune forme con tutti i parametri richiesti (upperLeftRow, upperLeftColumn, height, width, imageWidth, imageHeight)
            Shape shape1 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 50, 100);
            Shape shape2 = worksheet.Shapes.AddRectangle(6, 0, 2, 0, 50, 100);
            Shape shape3 = worksheet.Shapes.AddRectangle(3, 0, 5, 0, 50, 100);

            // Raggruppa le forme con i parametri corretti
            GroupShape group = worksheet.Shapes.Group(new Shape[] { shape1, shape2, shape3 });

            // Verifica se le forme sono in un gruppo
            Console.WriteLine("Shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("Shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("Shape3 IsInGroup: " + shape3.IsInGroup);
            Console.WriteLine("GroupShape IsInGroup: " + group.IsInGroup);

            // Aggiungi una forma non raggruppata
            Shape ungroupedShape = worksheet.Shapes.AddRectangle(10, 0, 2, 0, 50, 100);
            Console.WriteLine("Ungrouped shape IsInGroup: " + ungroupedShape.IsInGroup);

            // Salva il risultato
            workbook.Save("ShapePropertyIsInGroupDemo.xlsx");

            // Separa le forme e ottieni le forme non raggruppate dal gruppo
            group.Ungroup();
            Console.WriteLine("After ungrouping, shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("After ungrouping, shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("After ungrouping, shape3 IsInGroup: " + shape3.IsInGroup);

            // Salva il risultato
            workbook.Save("ShapePropertyIsInGroupDemo2.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


