---
title: "Cell.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt die Spaltennummer (nullbasiert) der Zelle zurück"
type: docs
url: /de/net/aspose.cells/cell/column/
---
## Cell.Column property

Liefert die Spaltennummer (nullbasiert) der Zelle.

```csharp
public int Column { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf Zellen und Demonstration der Column-Eigenschaft
            Cell cell1 = worksheet.Cells["A1"];
            Cell cell2 = worksheet.Cells["B2"];
            Cell cell3 = worksheet.Cells["C3"];

            // Werte und Formatierungen festlegen
            cell1.PutValue("Cell A1");
            cell2.PutValue("Cell B2");
            cell3.PutValue("Cell C3");

            // Demonstration der Verwendung der Column-Eigenschaft
            Console.WriteLine("Cell A1 is in column: " + cell1.Column);
            Console.WriteLine("Cell B2 is in column: " + cell2.Column);
            Console.WriteLine("Cell C3 is in column: " + cell3.Column);

            // Spaltenbreite mithilfe der Column-Eigenschaft ändern
            worksheet.Cells.Columns[cell1.Column].Width = 20;
            worksheet.Cells.Columns[cell2.Column].Width = 25;
            worksheet.Cells.Columns[cell3.Column].Width = 30;

            // Speichere die Arbeitsmappe
            workbook.Save("ColumnPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


