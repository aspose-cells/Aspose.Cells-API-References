---
title: "DataBarBorder.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBarBorder. Ottiene o imposta il colore dei bordi delle barre dati specificate da una regola di formattazione condizionale"
type: docs
url: /it/net/aspose.cells/databarborder/color/
---
## DataBarBorder.Color property

Ottiene o imposta il colore del bordo delle barre dei dati specificato da una regola di formattazione condizionale.

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
    public class DataBarBorderPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea una raccolta di condizioni di formattazione
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(new CellArea { StartRow = 2, StartColumn = 4, EndRow = 3, EndColumn = 6 });

            // Aggiungi una condizione di formattazione a barra dati
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Imposta le proprietà della barra dati
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Imposta le proprietà del bordo (dimostrando l'uso di Color)
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // Salva la cartella di lavoro
            workbook.Save("DataBarBorderColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar border color demo completed.");
        }
    }
}
```

### Vedi anche

* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


