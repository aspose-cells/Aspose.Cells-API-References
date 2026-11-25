---
title: "Worksheet.Zoom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400"
type: docs
url: /it/net/aspose.cells/worksheet/zoom/
---
## Worksheet.Zoom property

Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400.

```csharp
public int Zoom { get; set; }
```

### Osservazioni

Imposta prima il tipo di visualizzazione.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyZoomDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il fattore di zoom al 120%
            worksheet.Zoom = 120;
            
            // Visualizza il fattore di zoom corrente
            Console.WriteLine("Current worksheet zoom: " + worksheet.Zoom + "%");
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetZoomDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


