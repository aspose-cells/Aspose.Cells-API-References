---
title: "VerticalPageBreakCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VerticalPageBreakCollection. Rimuove l'elemento VPageBreak con un nome specificato"
type: docs
url: /it/net/aspose.cells/verticalpagebreakcollection/removeat/
---
## VerticalPageBreakCollection.RemoveAt method

Rimuove l'elemento VPageBreak con un nome specificato.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | Indice dell'elemento, a base zero. |

### Esempi

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

### Vedi anche

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


