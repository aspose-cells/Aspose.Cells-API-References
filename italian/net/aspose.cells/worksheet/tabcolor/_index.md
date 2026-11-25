---
title: "Worksheet.TabColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Rappresenta il colore della scheda del foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

Rappresenta il colore della scheda del foglio di lavoro.

```csharp
public Color TabColor { get; set; }
```

### Osservazioni

Questa funzionalità è supportata solo in ExcelXP (Excel2002) e versioni successive. Se salvi il file in formato Excel97 o Excel2000, verrà omessa.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il colore della scheda su rosso
            worksheet.TabColor = Color.Red;
            Console.WriteLine("Tab color set to: " + worksheet.TabColor);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Cancella il colore della scheda
            worksheet.TabColor = Color.Empty;
            Console.WriteLine("Tab color cleared: " + worksheet.TabColor.IsEmpty);
            
            // Salva la cartella di lavoro modificata
            workbook.Save("output_modified.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


