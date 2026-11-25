---
title: "Worksheet.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Worksheet property. Rappresenta se il foglio di lavoro è visibile"
type: docs
url: /it/net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Rappresenta se il foglio di lavoro è visibile.

```csharp
public bool IsVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi 3 fogli di lavoro
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Imposta il secondo foglio di lavoro come nascosto
            workbook.Worksheets[1].IsVisible = false;
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetVisibilityDemo.xlsx");
            
            // Visualizza lo stato di visibilità
            Console.WriteLine("Worksheet Visibility Status:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Console.WriteLine($"{workbook.Worksheets[i].Name}: {(workbook.Worksheets[i].IsVisible ? "Visible" : "Hidden")}");
            }
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


