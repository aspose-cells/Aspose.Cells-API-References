---
title: "Style.VerticalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene o imposta il tipo di allineamento verticale del testo in una cella"
type: docs
url: /it/net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

Ottiene o imposta il tipo di allineamento verticale del testo in una cella.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella A1
            Cell cell = worksheet.Cells["A1"];
            
            // Imposta il valore della cella
            cell.PutValue("Vertical Alignment Demo");
            
            // Accedi allo stile della cella
            Style style = cell.GetStyle();
            
            // Imposta l'allineamento verticale su Top
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("VerticalAlignmentDemo.xlsx");
            
            Console.WriteLine("Vertical alignment set to Top for cell A1.");
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


