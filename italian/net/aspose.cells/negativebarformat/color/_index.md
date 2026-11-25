---
title: "NegativeBarFormat.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà NegativeBarFormat. Ottiene o imposta un oggetto FormatColor che puoi usare per specificare il colore di riempimento per le barre dati negative"
type: docs
url: /it/net/aspose.cells/negativebarformat/color/
---
## NegativeBarFormat.Color property

Ottiene o imposta un oggetto FormatColor che puoi usare per specificare il colore di riempimento per le barre dati negative.

```csharp
public Color Color { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyColorDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Crea formattazione condizionale
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Configura le proprietà della barra dati
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Configura il formato della barra negativa
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Salva la cartella di lavoro
            workbook.Save("NegativeBarFormatColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("NegativeBarFormatPropertyColorDemo executed successfully.");
        }
    }
}
```

### Vedi anche

* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


