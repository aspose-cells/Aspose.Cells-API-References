---
title: "ShapeCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeCollection. Ottiene l'oggetto Shape all'indice specifico nella lista"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/item/
---
## ShapeCollection indexer (1 of 2)

Ottiene l'oggetto [`Shape`](../../shape/) all'indice specifico nella lista.

```csharp
public Shape this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcune forme al foglio di lavoro con i parametri corretti
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            worksheet.Shapes.AddLine(3, 0, 300, 100, 100, 100);

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Dimostrare la proprietà Item ottenendo la prima forma
            Shape firstShape = shapes[0];
            Console.WriteLine("First shape type: " + firstShape.Type);

            // Dimostrare la proprietà Item ottenendo la forma per ID
            Shape shapeById = shapes[2];
            Console.WriteLine("Shape with ID 2 type: " + shapeById.Type);
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ShapeCollection indexer (2 of 2)

Ottiene l'oggetto [`Shape`](../../shape/) per il nome della forma.

```csharp
public Shape this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome della forma. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi forme al foglio di lavoro
            ShapeCollection shapes = worksheet.Shapes;
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);
            shapes.AddOval(5, 0, 2, 0, 130, 130);
            
            // Accedi alle forme usando la proprietà Item
            Shape rectangle = shapes["Rectangle 1"];
            if (rectangle != null)
            {
                rectangle.FillFormat.ForeColor = System.Drawing.Color.Red;
            }
            
            Shape oval = shapes["Oval 2"];
            if (oval != null)
            {
                oval.FillFormat.ForeColor = System.Drawing.Color.Blue;
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ShapeCollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


