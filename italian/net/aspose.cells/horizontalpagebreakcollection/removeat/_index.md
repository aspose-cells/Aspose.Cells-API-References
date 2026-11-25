---
title: "HorizontalPageBreakCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo HorizontalPageBreakCollection. Rimuove l'elemento HPageBreak con un nome specificato"
type: docs
url: /it/net/aspose.cells/horizontalpagebreakcollection/removeat/
---
## HorizontalPageBreakCollection.RemoveAt method

Rimuove l'elemento HPageBreak con un nome specificato.

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
    public class HorizontalPageBreakCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            worksheet.HorizontalPageBreaks.Add(15);
            
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


