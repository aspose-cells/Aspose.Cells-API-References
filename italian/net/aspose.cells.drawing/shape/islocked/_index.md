---
title: "Shape.IsLocked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. True indica che l'oggetto non può essere modificato quando il foglio è protetto. Nota che questo valore ha senso solo se il foglio di lavoro o gli oggetti nel foglio di lavoro sono protetti"
type: docs
url: /it/net/aspose.cells.drawing/shape/islocked/
---
## Shape.IsLocked property

True indica che l'oggetto non può essere modificato quando il foglio è protetto. Nota che questo valore è significativo solo se il foglio di lavoro o gli oggetti nel foglio di lavoro sono protetti.

```csharp
public bool IsLocked { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Proteggi il foglio di lavoro
            worksheet.Protect(ProtectionType.All);

            // Dimostra il blocco/sblocco della forma
            Console.WriteLine("Original IsLocked state: " + shape.IsLocked);

            // Sblocca la forma
            shape.IsLocked = false;
            Console.WriteLine("After unlocking, IsLocked state: " + shape.IsLocked);

            // Blocca la forma
            shape.IsLocked = true;
            Console.WriteLine("After locking, IsLocked state: " + shape.IsLocked);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


