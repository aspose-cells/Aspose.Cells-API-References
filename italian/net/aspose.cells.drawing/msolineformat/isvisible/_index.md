---
title: "MsoLineFormat.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormat. Indica se l'oggetto è visibile"
type: docs
url: /it/net/aspose.cells.drawing/msolineformat/isvisible/
---
## MsoLineFormat.IsVisible property

Indica se l'oggetto è visibile.

```csharp
public bool IsVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con bordo visibile
            var shape1 = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape1.LineFormat.IsVisible = true;

            // Aggiungi una forma ovale con bordo invisibile
            var shape2 = worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            shape2.LineFormat.IsVisible = false;

            // Verifica e stampa i valori della proprietà IsVisible
            Console.WriteLine("Rectangle border visible: " + shape1.LineFormat.IsVisible);
            Console.WriteLine("Oval border visible: " + shape2.LineFormat.IsVisible);

            // Salva la cartella di lavoro
            workbook.Save("MsoLineFormat_IsVisible_Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


