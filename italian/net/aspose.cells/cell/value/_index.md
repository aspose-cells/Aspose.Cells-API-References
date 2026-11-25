---
title: "Cell.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottiene/imposta il valore contenuto in questa cella"
type: docs
url: /it/net/aspose.cells/cell/value/
---
## Cell.Value property

Ottiene/imposta il valore contenuto in questa cella.

```csharp
public object Value { get; set; }
```

### Osservazioni

Tipo possibile:

null,

Boolean,

DateTime,

Double,

Integer

String.

Per un valore int, potrebbe essere restituito come un oggetto Integer o un oggetto Double. Inoltre non c'è alcuna garanzia che il valore restituito rimanga sempre dello stesso tipo di oggetto.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta i valori usando la proprietà Value
            cells[0, 0].Value = "Product ID";
            cells[0, 1].Value = "Product Name";
            
            // Dimostra i valori null
            cells[0, 2].Value = null;
            cells[1, 0].Value = null;
            cells[1, 1].Value = null;
            cells[1, 2].Value = null;

            // Visualizza i valori
            Console.WriteLine("Cell[0,0] Value: " + cells[0, 0].Value);
            Console.WriteLine("Cell[0,1] Value: " + cells[0, 1].Value);
            Console.WriteLine("Cell[0,2] Value: " + (cells[0, 2].Value == null ? "null" : cells[0, 2].Value));
            Console.WriteLine("Cell[1,0] Value: " + (cells[1, 0].Value == null ? "null" : cells[1, 0].Value));
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


