---
title: "Worksheet.VerticalPageBreaks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene la colección VerticalPageBreakCollection"
type: docs
url: /es/net/aspose.cells/worksheet/verticalpagebreaks/
---
## Worksheet.VerticalPageBreaks property

Obtiene la colección [`VerticalPageBreakCollection`](../../verticalpagebreakcollection/).

```csharp
public VerticalPageBreakCollection VerticalPageBreaks { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVerticalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Agregue diferentes tipos de saltos de página verticales
            verticalPageBreaks.Add(0, 10, 2);
            verticalPageBreaks.Add(4);
            verticalPageBreaks.Add(5, 3);
            verticalPageBreaks.Add("G5");

            // Elimine un salto
            verticalPageBreaks.RemoveAt(1);

            // Imprima la información del salto
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Break {i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Ver también

* class [VerticalPageBreakCollection](../../verticalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


