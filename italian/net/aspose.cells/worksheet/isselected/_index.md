---
title: "Worksheet.IsSelected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta"
type: docs
url: /it/net/aspose.cells/worksheet/isselected/
---
## Worksheet.IsSelected property

Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta.

```csharp
public bool IsSelected { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsSelectedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un secondo foglio di lavoro
            workbook.Worksheets.Add("Sheet2");
            
            // Ottieni il primo foglio di lavoro
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "FirstSheet";
            
            // Ottieni il secondo foglio di lavoro
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet2.Name = "SecondSheet";
            
            // Dimostra la proprietà IsSelected
            Console.WriteLine("Before selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Seleziona il secondo foglio di lavoro
            worksheet2.IsSelected = true;
            workbook.Worksheets.ActiveSheetIndex = worksheet2.Index;
            
            Console.WriteLine("\nAfter selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetSelectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


