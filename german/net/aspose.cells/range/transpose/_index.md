---
title: "Range.Transpose"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Transponiert (dreht) Daten von Zeilen zu Spalten oder umgekehrt"
type: docs
url: /de/net/aspose.cells/range/transpose/
---
## Range.Transpose method

Transponiert (dreht) Daten von Zeilen zu Spalten oder umgekehrt.

```csharp
public void Transpose()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodTransposeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fülle Beispieldaten in einen 3 × 3‑Bereich (A1:C3)
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].PutValue(6);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["C3"].PutValue(9);
            
            // Erstelle einen Bereich (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            
            // Transponiere den Bereich
            range.Transpose();
            
            // Speichere die Arbeitsmappe
            workbook.Save("TransposedOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


