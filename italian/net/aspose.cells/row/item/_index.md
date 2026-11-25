---
title: "Row.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Row. Ottiene la cella"
type: docs
url: /it/net/aspose.cells/row/item/
---
## Row indexer

Ottiene la cella.

```csharp
public Cell this[int column] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| colonna | L'indice di colonna |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Accedi alla prima riga
            Row row = sheet.Cells.Rows[0];
            
            // Imposta contenuto HTML con diversi stili di colore
            row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
            row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
            
            // Dimostra l'uso della proprietà Item e visualizza i colori
            Console.WriteLine("Cell 0 Font Color: " + row[0].GetStyle().Font.Color.Name);
            Console.WriteLine("Cell 1 Font Color: " + row[1].GetStyle().Font.Color.Name);
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


