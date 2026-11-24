---
title: "Cell.Worksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt das übergeordnete Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells/cell/worksheet/
---
## Cell.Worksheet property

Ermittelt das übergeordnete Arbeitsblatt.

```csharp
public Worksheet Worksheet { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Greifen Sie auf eine Zelle zu und demonstrieren Sie die Worksheet-Eigenschaft
            Cell cell = worksheet.Cells["A3"];
            
            // Zeigen Sie Arbeitsblattinformationen über die Worksheet-Eigenschaft der Zelle an
            Console.WriteLine("Cell A3 is in worksheet: " + cell.Worksheet.Name);
            Console.WriteLine("Calculation result in A3: " + cell.Value);
            
            // Fügen Sie ein weiteres Arbeitsblatt hinzu und demonstrieren Sie den Querverweis zwischen Arbeitsblättern
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=A3");
            
            // Greifen Sie auf die Zelle in Sheet2 zu und zeigen Sie ihr Arbeitsblatt
            Cell crossSheetCell = sheet2.Cells["B1"];
            Console.WriteLine("Cell B1 is in worksheet: " + crossSheetCell.Worksheet.Name);
            Console.WriteLine("Cross-sheet reference in B1: " + crossSheetCell.Value);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


