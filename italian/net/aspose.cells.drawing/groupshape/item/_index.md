---
title: "GroupShape.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GroupShape property. Ottiene la forma figlia per indice"
type: docs
url: /it/net/aspose.cells.drawing/groupshape/item/
---
## GroupShape indexer

Ottiene la forma figlia per indice.

```csharp
public Shape this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | l'indice della forma figlia. |

### Valore di ritorno

restituisce la forma figlia.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapePropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due forme rettangolari
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Raggruppa le forme
            Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
            GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);

            // Accedi e visualizza le proprietà della prima forma
            Shape firstShape = groupShape[0];
            Console.WriteLine($"First shape initial name: {firstShape.Name}");
            Console.WriteLine($"First shape initial text: {firstShape.Text}");

            // Modifica le proprietà della prima forma tramite l'accesso a Item
            firstShape.Name = "ModifiedRectangle1";
            firstShape.Text = "First Grouped Shape";

            // Accedi e modifica la seconda forma direttamente tramite l'indicizzatore
            groupShape[1].Text = "Second Grouped Shape";

            // Verifica le modifiche
            Console.WriteLine($"\nFirst shape updated name: {groupShape[0].Name}");
            Console.WriteLine($"First shape updated text: {groupShape[0].Text}");
            Console.WriteLine($"Second shape updated text: {groupShape[1].Text}");

            // Salvare la cartella di lavoro modificata
            workbook.Save("GroupShapePropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


