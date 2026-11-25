---
title: "Worksheet.ViewType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene e imposta il tipo di visualizzazione"
type: docs
url: /it/net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Ottiene e imposta il tipo di visualizzazione.

```csharp
public ViewType ViewType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyViewTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il tipo di visualizzazione su PageLayoutView e abilita il righello
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsRulerVisible = true;
            
            // Aggiungi del contenuto di esempio per dimostrare la visualizzazione
            worksheet.Cells["A1"].PutValue("Page Layout View Demo");
            worksheet.Cells["A2"].PutValue("Ruler is visible in this view");
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetViewTypeDemo.xlsx");
            
            Console.WriteLine("Worksheet ViewType demo completed successfully.");
        }
    }
}
```

### Vedi anche

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


