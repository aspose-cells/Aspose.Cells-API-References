---
title: "VerticalPageBreakCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VerticalPageBreakCollection. Elimina el elemento VPageBreak con un nombre especificado"
type: docs
url: /es/net/aspose.cells/verticalpagebreakcollection/removeat/
---
## VerticalPageBreakCollection.RemoveAt method

Elimina el elemento VPageBreak con un nombre especificado.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | Índice del elemento, basado en cero. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            verticalPageBreaks.Add(0, 10, 2);
            verticalPageBreaks.Add(4);
            verticalPageBreaks.Add(5, 3);
            verticalPageBreaks.Add("G5");

            verticalPageBreaks.RemoveAt(1);

            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: Column = {vpb.Column}, StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}");
            }

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


