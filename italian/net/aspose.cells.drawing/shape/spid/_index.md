---
title: "Shape.Spid"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Specifica un identificatore stringa opzionale che un'applicazione può utilizzare per identificare la forma specifica"
type: docs
url: /it/net/aspose.cells.drawing/shape/spid/
---
## Shape.Spid property

Specifica un identificatore stringa opzionale che un'applicazione può utilizzare per identificare la forma specifica.

```csharp
public string Spid { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySpidDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare al foglio di lavoro con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Ottieni e visualizza la proprietà Spid della forma
            string spid = shape.Spid;
            Console.WriteLine("Shape SPID: " + spid);

            // Salva la cartella di lavoro
            workbook.Save("ShapePropertySpidDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


