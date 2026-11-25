---
title: "Worksheet.IsGridlinesVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene o imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

Ottiene o imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsGridlinesVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la visibilità delle linee della griglia su true
            worksheet.IsGridlinesVisible = true;
            
            // Aggiungi alcuni dati di esempio per vedere le linee della griglia
            worksheet.Cells["A1"].PutValue("Gridlines Visible Example");
            worksheet.Cells["A2"].PutValue("This worksheet shows gridlines");
            
            // Adatta automaticamente le colonne per una migliore visibilità
            worksheet.AutoFitColumns();
            
            // Salva la cartella di lavoro
            workbook.Save("GridlinesVisibleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


