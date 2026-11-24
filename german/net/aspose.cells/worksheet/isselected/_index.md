---
title: "Worksheet.IsSelected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob dieses Arbeitsblatt ausgewählt ist, wenn die Arbeitsmappe geöffnet wird"
type: docs
url: /de/net/aspose.cells/worksheet/isselected/
---
## Worksheet.IsSelected property

Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist.

```csharp
public bool IsSelected { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsSelectedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge ein zweites Arbeitsblatt hinzu
            workbook.Worksheets.Add("Sheet2");
            
            // Hole das erste Arbeitsblatt
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "FirstSheet";
            
            // Hole das zweite Arbeitsblatt
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet2.Name = "SecondSheet";
            
            // Demonstriere die IsSelected-Eigenschaft
            Console.WriteLine("Before selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Wähle das zweite Arbeitsblatt aus
            worksheet2.IsSelected = true;
            workbook.Worksheets.ActiveSheetIndex = worksheet2.Index;
            
            Console.WriteLine("\nAfter selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetSelectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


