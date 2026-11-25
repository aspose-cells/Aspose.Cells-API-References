---
title: "ColorScale.MinCfvo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ColorScale. Ottieni o imposta questo oggetto valore minimo di ColorScale. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Max."
type: docs
url: /it/net/aspose.cells/colorscale/mincfvo/
---
## ColorScale.MinCfvo property

Ottieni o imposta l'oggetto valore minimo di questo ColorScale. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Max su di esso.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinCfvoDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Crea una formattazione condizionale a scala di colore
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Aggiungi scala di colore
            int csIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            ColorScale cs = fcc[csIndex].ColorScale;

            // Imposta le proprietà MinCfvo
            cs.MinCfvo.Type = FormatConditionValueType.Min;
            cs.MinCfvo.Value = "0";
            cs.MinColor = System.Drawing.Color.Red;

            // Imposta le proprietà MidCfvo
            cs.MidCfvo.Type = FormatConditionValueType.Percentile;
            cs.MidCfvo.Value = "50";
            cs.MidColor = System.Drawing.Color.Yellow;

            // Imposta le proprietà MaxCfvo
            cs.MaxCfvo.Type = FormatConditionValueType.Max;
            cs.MaxCfvo.Value = "0";
            cs.MaxColor = System.Drawing.Color.Green;

            // Salva la cartella di lavoro
            workbook.Save("ColorScaleMinCfvoDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


