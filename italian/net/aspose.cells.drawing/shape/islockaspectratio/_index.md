---
title: "Shape.IsLockAspectRatio"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. True indica che il rapporto d'aspetto della forma è bloccato"
type: docs
url: /it/net/aspose.cells.drawing/shape/islockaspectratio/
---
## Shape.IsLockAspectRatio property

True indica che il rapporto d'aspetto della forma è bloccato.

```csharp
[Obsolete("Use Shape.IsAspectRatioLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLockAspectRatio { get; set; }
```

### Osservazioni

Solo per immagini e oggetti Ole. NOTA: questo membro è ora obsoleto. Invece, utilizzare la proprietà Shape.IsAspectRatioLocked. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockAspectRatioDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Blocca rapporto d'aspetto
            shape.IsLockAspectRatio = true;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);

            // Sblocca rapporto d'aspetto
            shape.IsLockAspectRatio = false;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


