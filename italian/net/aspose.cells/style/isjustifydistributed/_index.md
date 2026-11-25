---
title: "Style.IsJustifyDistributed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se l'allineamento giustificato o distribuito delle celle deve essere usato sull'ultima riga di testo"
type: docs
url: /it/net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Indica se l'allineamento giustificato o distribuito delle celle deve essere usato sull'ultima riga di testo.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Osservazioni

Questo è tipico per gli allineamenti dell'Asia orientale ma non è tipico in altri contesti. Funziona solo quando è attivo l'allineamento distribuito.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsJustifyDistributedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella B3 e imposta il suo testo
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("Sample Text");

            // Ottieni lo stile della cella e imposta IsJustifyDistributed su true
            Style style = cell.GetStyle();
            style.IsJustifyDistributed = true;
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            // Verifica la proprietà
            Console.WriteLine("IsJustifyDistributed: " + cell.GetStyle().IsJustifyDistributed);
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


