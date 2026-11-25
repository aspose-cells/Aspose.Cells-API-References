---
title: "HorizontalPageBreak.StartColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HorizontalPageBreak. Restituisce l'indice della colonna iniziale di questa interruzione di pagina orizzontale"
type: docs
url: /it/net/aspose.cells/horizontalpagebreak/startcolumn/
---
## HorizontalPageBreak.StartColumn property

Restituisce l'indice della colonna iniziale di questa interruzione di pagina orizzontale.

```csharp
public int StartColumn { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyStartColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi interruzioni di pagina in colonne diverse per dimostrare StartColumn
            int index1 = worksheet.HorizontalPageBreaks.Add("Y30");
            int index2 = worksheet.HorizontalPageBreaks.Add("B30");
            
            HorizontalPageBreak hPageBreak1 = worksheet.HorizontalPageBreaks[index1];
            HorizontalPageBreak hPageBreak2 = worksheet.HorizontalPageBreaks[index2];
            
            Console.WriteLine($"First Break Start Column: {hPageBreak1.StartColumn}");
            Console.WriteLine($"Second Break Start Column: {hPageBreak2.StartColumn}");
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


