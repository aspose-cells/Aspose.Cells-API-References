---
title: "Worksheet.IsSelected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger om detta kalkylblad är markerat när arbetsboken öppnas"
type: docs
url: /sv/net/aspose.cells/worksheet/isselected/
---
## Worksheet.IsSelected property

Anger om detta kalkylblad är valt när arbetsboken öppnas.

```csharp
public bool IsSelected { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsSelectedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett andra kalkylblad
            workbook.Worksheets.Add("Sheet2");
            
            // Hämta det första kalkylbladet
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "FirstSheet";
            
            // Hämta det andra kalkylbladet
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet2.Name = "SecondSheet";
            
            // Demonstrera IsSelected-egenskapen
            Console.WriteLine("Before selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Markera det andra kalkylbladet
            worksheet2.IsSelected = true;
            workbook.Worksheets.ActiveSheetIndex = worksheet2.Index;
            
            Console.WriteLine("\nAfter selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Spara arbetsboken
            workbook.Save("WorksheetSelectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


