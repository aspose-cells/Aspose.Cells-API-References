---
title: "NegativeBarFormat.ColorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà NegativeBarFormat. Ottiene o imposta se utilizzare lo stesso colore di riempimento dei data bar positivi"
type: docs
url: /it/net/aspose.cells/negativebarformat/colortype/
---
## NegativeBarFormat.ColorType property

Ottiene o imposta se utilizzare lo stesso colore di riempimento delle barre dati positive.

```csharp
public DataBarNegativeColorType ColorType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-15);
            sheet.Cells["F4"].PutValue(25);
            sheet.Cells["G3"].PutValue(-5);
            sheet.Cells["G4"].PutValue(15);

            // Crea intervallo di formattazione condizionale
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Aggiungi formattazione condizionale della barra dati
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(area);
            
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Imposta le proprietà della barra dati
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            
            // Configura il formato della barra negativa
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Salva la cartella di lavoro
            workbook.Save("NegativeBarFormatDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Demo completed. File saved with negative bar formatting.");
        }
    }
}
```

### Vedi anche

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


