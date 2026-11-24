---
title: "Range.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt das Cell-Objekt in diesem Bereich zurück"
type: docs
url: /de/net/aspose.cells/range/item/
---
## Range indexer

Gibt ein [`Cell`](../../cell/)-Objekt in diesem Bereich zurück.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| rowOffset | Zeilenversatz in diesem Bereich, nullbasiert. |
| columnOffset | Spaltenversatz in diesem Bereich, nullbasiert. |

### Rückgabewert

[`Cell`](../../cell/) object.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten
            DataTable dt = new DataTable();
            dt.Columns.Add("Id", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Rows.Add(1001, "Item 1");
            dt.Rows.Add(1002, "Item 2");

            // Erstellen Sie einen Bereich und demonstrieren Sie die Item-Eigenschaft
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B3");
            
            // Setzen Sie Kopfzeilen mithilfe der Item-Eigenschaft
            range[0, 0].PutValue("Id");
            range[0, 1].PutValue("Name");

            // Füllen Sie Daten mithilfe der Item-Eigenschaft
            for (int i = 0; i < dt.Rows.Count; i++)
            {
                range[i + 1, 0].PutValue(dt.Rows[i]["Id"]);
                range[i + 1, 1].PutValue(dt.Rows[i]["Name"]);
            }

            // Formatieren Sie die Kopfzeilenzeile mithilfe der Item-Eigenschaft
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.FromArgb(0, 176, 80);
            range[0, 0].SetStyle(style);
            range[0, 1].SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("RangePropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


