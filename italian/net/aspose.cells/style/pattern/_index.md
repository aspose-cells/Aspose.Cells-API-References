---
title: "Style.Pattern"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene o imposta il tipo di motivo di sfondo della cella"
type: docs
url: /it/net/aspose.cells/style/pattern/
---
## Style.Pattern property

Ottiene o imposta il tipo di modello di sfondo della cella.

```csharp
public BackgroundType Pattern { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyPatternDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Accedi alla cella e ottieni il suo stile
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            
            // Imposta il motivo e il colore di primo piano
            style.Pattern = BackgroundType.Gray50;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            
            // Applica lo stile alla cella
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("PatternPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


