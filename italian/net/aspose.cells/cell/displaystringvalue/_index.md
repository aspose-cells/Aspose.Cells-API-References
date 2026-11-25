---
title: "Cell.DisplayStringValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Restituisce il valore stringa formattato di questa cella secondo lo stile di visualizzazione della cella"
type: docs
url: /it/net/aspose.cells/cell/displaystringvalue/
---
## Cell.DisplayStringValue property

Restituisce il valore stringa formattato di questa cella secondo lo stile di visualizzazione della cella.

```csharp
public string DisplayStringValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDisplayStringValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Primo esempio
            Style style = cell.GetStyle();
            style.Custom = "# ##/##\\\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: 3"
            
            // Secondo esempio
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3
            
            // Terzo esempio
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Quarto esempio con valore decimale
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1b c11d/e47f
            
            // Quinto esempio con formato modificato
            style.Custom = "\"a\"#\"b\"\"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Sesto esempio con valore decimale
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1bc11d/e47f
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


