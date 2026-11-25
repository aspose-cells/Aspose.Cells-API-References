---
title: "ColorScale.MidCfvo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ColorScale. Ottieni o imposta questo oggetto valore medio di ColorScale. Non è possibile impostare CFValueObject con tipo FormatConditionValueType.Max o FormatConditionValueType.Min."
type: docs
url: /it/net/aspose.cells/colorscale/midcfvo/
---
## ColorScale.MidCfvo property

Ottieni o imposta l'oggetto valore medio di questo ColorScale. Non è possibile impostare CFValueObject con tipo FormatConditionValueType.Max o FormatConditionValueType.Min su di esso.

```csharp
public ConditionalFormattingValue MidCfvo { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMidCfvoDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Aggiungi una formattazione condizionale a scala di colore
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            int conditionIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            
            // Imposta il valore del punto medio per la scala di colore
            ColorScale colorScale = fcc[conditionIndex].ColorScale;
            colorScale.MidCfvo.Type = FormatConditionValueType.Number;
            colorScale.MidCfvo.Value = 50;

            // Salva la cartella di lavoro
            workbook.Save("ColorScalePropertyMidCfvoDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


