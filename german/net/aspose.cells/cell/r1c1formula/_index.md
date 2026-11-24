---
title: "Cell.R1C1Formula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt eine R1C1-Formel der Zelle zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

Gibt eine R1C1-Formel des [`Cell`](../) zurück oder legt sie fest.

```csharp
public string R1C1Formula { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyR1C1FormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze den A1-Wert
            worksheet.Cells["A1"].PutValue(10);
            
            // Setze den B1-Wert
            worksheet.Cells["B1"].PutValue(20);
            
            // Setze die C1-Formel in A1-Notation
            worksheet.Cells["C1"].Formula = "=A1+B1";
            
            // Abrufen und Anzeigen der R1C1-Formel
            string r1c1Formula = worksheet.Cells["C1"].R1C1Formula;
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
            
            // Setze die D1-Formel in R1C1-Notation
            worksheet.Cells["D1"].R1C1Formula = "=RC[-3]+RC[-2]";
            
            // Abrufen und Anzeigen der A1-Formel
            string a1Formula = worksheet.Cells["D1"].Formula;
            Console.WriteLine("A1 Formula: " + a1Formula);
            
            // Speichere die Arbeitsmappe
            workbook.Save("R1C1FormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


