---
title: "Row.IsBlank"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Row. Indica se la riga contiene dei dati"
type: docs
url: /it/net/aspose.cells/row/isblank/
---
## Row.IsBlank property

Indica se la riga contiene dati

```csharp
public bool IsBlank { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsBlankDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la prima riga (inizialmente vuota)
            Row row1 = worksheet.Cells.Rows[0];
            Console.WriteLine("Row 1 IsBlank: " + row1.IsBlank); // True
            
            // Aggiungi dati alla prima riga
            worksheet.Cells["A1"].PutValue("Test");
            Console.WriteLine("Row 1 IsBlank after adding data: " + row1.IsBlank); // False
            
            // Crea un'altra riga vuota
            Row row2 = worksheet.Cells.Rows[1];
            Console.WriteLine("Row 2 IsBlank: " + row2.IsBlank); // True
            
            // Confronta lo stato di vuoto della riga
            Console.WriteLine("Rows have same IsBlank status: " + (row1.IsBlank == row2.IsBlank)); // False
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


