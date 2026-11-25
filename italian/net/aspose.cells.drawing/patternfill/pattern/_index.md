---
title: "PatternFill.Pattern"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PatternFill. Ottiene o imposta il tipo di pattern di riempimento"
type: docs
url: /it/net/aspose.cells.drawing/patternfill/pattern/
---
## PatternFill.Pattern property

Ottiene o imposta il tipo di pattern di riempimento

```csharp
public FillPattern Pattern { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PatternFillPropertyPatternDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Imposta il pattern di riempimento per la prima serie
            chart.NSeries[0].Area.FillFormat.FillType = FillType.Pattern;
            chart.NSeries[0].Area.FillFormat.PatternFill.Pattern = FillPattern.WideDownwardDiagonal;
            
            // Salva la cartella di lavoro
            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FillPattern](../../fillpattern/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


