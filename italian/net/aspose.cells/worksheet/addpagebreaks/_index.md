---
title: "Worksheet.AddPageBreaks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Aggiunge interruzione di pagina"
type: docs
url: /it/net/aspose.cells/worksheet/addpagebreaks/
---
## Worksheet.AddPageBreaks method

Aggiunge un'interruzione di pagina.

```csharp
public void AddPageBreaks(string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String |  |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAddPageBreaksWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi interruzione di pagina orizzontale alla riga 1 (B2)
            worksheet.AddPageBreaks("B2");

            // Aggiungi interruzione di pagina orizzontale alla riga 9 (B10)
            worksheet.AddPageBreaks("B10");

            // Verifica che la prima interruzione di pagina sia stata aggiunta alla riga 1
            Console.WriteLine("First page break row: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


