---
title: "Range.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Ottiene l'oggetto Cell in questo intervallo"
type: docs
url: /it/net/aspose.cells/range/item/
---
## Range indexer

Ottiene l'oggetto [`Cell`](../../cell/) in questo intervallo.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| rowOffset | Offset di riga in questo intervallo, basato su zero. |
| columnOffset | Offset di colonna in questo intervallo, basato su zero. |

### Valore di ritorno

[`Cell`](../../cell/) object.

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangePropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio
            DataTable dt = new DataTable();
            dt.Columns.Add("Id", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Rows.Add(1001, "Item 1");
            dt.Rows.Add(1002, "Item 2");

            // Crea un intervallo e dimostra la proprietà Item
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B3");
            
            // Imposta le intestazioni usando la proprietà Item
            range[0, 0].PutValue("Id");
            range[0, 1].PutValue("Name");

            // Compila i dati usando la proprietà Item
            for (int i = 0; i < dt.Rows.Count; i++)
            {
                range[i + 1, 0].PutValue(dt.Rows[i]["Id"]);
                range[i + 1, 1].PutValue(dt.Rows[i]["Name"]);
            }

            // Formatta la riga di intestazione usando la proprietà Item
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.FromArgb(0, 176, 80);
            range[0, 0].SetStyle(style);
            range[0, 1].SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("RangePropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


