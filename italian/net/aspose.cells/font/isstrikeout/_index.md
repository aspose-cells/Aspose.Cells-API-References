---
title: "Font.IsStrikeout"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene o imposta un valore che indica se il carattere è barrato singolarmente"
type: docs
url: /it/net/aspose.cells/font/isstrikeout/
---
## Font.IsStrikeout property

Ottiene o imposta un valore che indica se il carattere è barrato singolo.

```csharp
public bool IsStrikeout { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsStrikeoutDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Metodo 1: Imposta il barrato direttamente tramite lo stile
            Cell cell1 = worksheet.Cells["A1"];
            Style style1 = cell1.GetStyle();
            style1.Font.IsStrikeout = true;
            cell1.SetStyle(style1);
            cell1.PutValue("Strikeout Text (Style)");
            
            // Metodo 2: Imposta il barrato tramite HTML
            Cell cell2 = worksheet.Cells["A2"];
            cell2.HtmlString = "<s>Strikeout Text (HTML)</s>";
            
            // Verifica la proprietà di barrato
            Console.WriteLine("A1 IsStrikeout: " + cell1.GetStyle().Font.IsStrikeout);
            Console.WriteLine("A2 IsStrikeout: " + cell2.GetStyle().Font.IsStrikeout);
            
            // Salva per la verifica
            workbook.Save("FontStrikeoutDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


