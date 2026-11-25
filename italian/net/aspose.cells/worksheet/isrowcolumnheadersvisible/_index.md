---
title: "Worksheet.IsRowColumnHeadersVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Worksheet property. Ottiene o imposta un valore che indica se il foglio di lavoro visualizzerà le intestazioni di righe e colonne. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/worksheet/isrowcolumnheadersvisible/
---
## Worksheet.IsRowColumnHeadersVisible property

Ottiene o imposta un valore che indica se il foglio di lavoro visualizzerà le intestazioni di righe e colonne. Il valore predefinito è true.

```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRowColumnHeadersVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la visibilità delle intestazioni di righe e colonne su false
            worksheet.IsRowColumnHeadersVisible = false;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare la proprietà
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Restituisci il valore della proprietà
            Console.WriteLine("Row and Column Headers Visible: " + loadedWorksheet.IsRowColumnHeadersVisible);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


