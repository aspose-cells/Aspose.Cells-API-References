---
title: "Row.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Eigenschaft. Gibt die Zelle zurück"
type: docs
url: /de/net/aspose.cells/row/item/
---
## Row indexer

Gibt die Zelle zurück.

```csharp
public Cell this[int column] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| column | Der Spalten‑Index |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Zeile zu
            Row row = sheet.Cells.Rows[0];
            
            // Setze HTML-Inhalt mit verschiedenen Farb‑Stilen
            row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
            row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
            
            // Demonstriere die Verwendung der Item‑Eigenschaft und gib die Farben aus
            Console.WriteLine("Cell 0 Font Color: " + row[0].GetStyle().Font.Color.Name);
            Console.WriteLine("Cell 1 Font Color: " + row[1].GetStyle().Font.Color.Name);
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


