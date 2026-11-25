---
title: "Style.IsNumberFormatApplied"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se la formattazione numerica deve essere applicata"
type: docs
url: /it/net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

Indica se la formattazione numerica deve essere applicata.

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### Osservazioni

Solo per stile con nome.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsNumberFormatAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea uno stile con formato numerico
            Style style = workbook.CreateStyle();
            style.Number = 14; // Format as "m/d/yyyy"
            style.IsNumberFormatApplied = true;
            
            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Verifica che il formato numerico sia applicato
            Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
            Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


