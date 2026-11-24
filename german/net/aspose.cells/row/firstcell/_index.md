---
title: "Row.FirstCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row Eigenschaft. Gibt das erste Zellenobjekt in der Zeile zurück"
type: docs
url: /de/net/aspose.cells/row/firstcell/
---
## Row.FirstCell property

Gibt das erste Zellenobjekt in der Zeile zurück.

```csharp
public Cell FirstCell { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Daten zu Zellen in der ersten Zeile hinzufügen
            worksheet.Cells["A1"].PutValue("First Cell");
            worksheet.Cells["B1"].PutValue("Second Cell");
            worksheet.Cells["C1"].PutValue("Third Cell");
            
            // Rufen Sie die erste Zeile ab
            Row row = worksheet.Cells.Rows[0];
            
            // Demonstriere die FirstCell-Eigenschaft
            Cell firstCell = row.FirstCell;
            Console.WriteLine("First cell in row: " + firstCell.Name + " with value: " + firstCell.StringValue);
            
            // Modifiziere die erste Zelle
            firstCell.PutValue("Modified First Cell");
            Console.WriteLine("Updated first cell value: " + firstCell.StringValue);
            
            // Speichere die Arbeitsmappe
            workbook.Save("RowFirstCellDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


