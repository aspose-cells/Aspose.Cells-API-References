---
title: "Cells.AddRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Aggiunge un riferimento a un oggetto range alle celle"
type: docs
url: /it/net/aspose.cells/cells/addrange/
---
## Cells.AddRange method

Aggiunge un riferimento a un oggetto range alle celle.

```csharp
public void AddRange(Range rangeObject)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rangeObject | Intervallo | L'oggetto range sarà contenuto nelle celle |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodAddRangeWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta alcuni dati di esempio nel range
            cells["A1"].PutValue("A1");
            cells["A2"].PutValue("A2");
            cells["B1"].PutValue("B1");
            cells["B2"].PutValue("B2");

            // Crea un range e aggiungilo usando AddRange
            Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
            cells.AddRange(range);

            // Modifica il foglio di lavoro per dimostrare l'espansione del range
            cells.InsertRow(1);
            cells.InsertColumn(1);

            Console.WriteLine($"Range now has {range.RowCount} rows and {range.ColumnCount} columns");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


