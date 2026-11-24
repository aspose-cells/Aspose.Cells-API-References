---
title: "Range.RefersTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt die Bezugnahme der Bereiche zurück"
type: docs
url: /de/net/aspose.cells/range/refersto/
---
## Range.RefersTo property

Liefert das 'refers to' des Bereichs.

```csharp
public string RefersTo { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Benannten Bereich erstellen
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            
            // Setze die RefersTo-Eigenschaft für den benannten Bereich
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Erhalte die durch den Namen referenzierten Bereiche
            Aspose.Cells.Range[] ranges = name.GetRanges();
            
            // Zeige die RefersTo-Eigenschaft des ersten Bereichs an
            Console.WriteLine("Named range refers to: " + ranges[0].RefersTo);
            
            // Erstelle eine Formel, die den benannten Bereich verwendet
            worksheet.Cells["B1"].Formula = "=SUM(MyRange)";
            
            // Formel berechnen
            Console.WriteLine("Sum of named range: " + worksheet.Cells["B1"].Value);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


