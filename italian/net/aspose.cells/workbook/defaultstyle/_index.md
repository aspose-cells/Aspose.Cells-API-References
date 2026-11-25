---
title: "Workbook.DefaultStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene o imposta l'oggetto Style predefinito della cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Ottiene o imposta l'oggetto [`Style`](../../style/) predefinito della cartella di lavoro.

```csharp
public Style DefaultStyle { get; set; }
```

### Osservazioni

La proprietà DefaultStyle è utile per implementare uno Style per l'intero Workbook.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDefaultStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Ottieni lo Style predefinito e modifica il suo carattere
            Style defaultStyle = workbook.DefaultStyle;
            defaultStyle.Font.Name = "Tahoma";
            defaultStyle.Font.Size = 12;
            
            // Applica lo Style modificato nuovamente come predefinito
            workbook.DefaultStyle = defaultStyle;
            
            // Crea un foglio di lavoro e aggiungi del testo con lo Style predefinito
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This text uses the default Tahoma font");
            
            // Salva la cartella di lavoro
            workbook.Save("DefaultStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


