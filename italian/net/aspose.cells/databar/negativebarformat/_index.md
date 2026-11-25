---
title: "DataBar.NegativeBarFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Ottiene l'oggetto NegativeBarFormat associato a una regola di formattazione condizionale della barra dati"
type: docs
url: /it/net/aspose.cells/databar/negativebarformat/
---
## DataBar.NegativeBarFormat property

Ottiene l'oggetto NegativeBarFormat associato a una regola di formattazione condizionale della DataBar.

```csharp
public NegativeBarFormat NegativeBarFormat { get; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyNegativeBarFormatDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con valori negativi
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Aggiungi formattazione condizionale della barra dati
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = sheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Imposta le proprietà della barra dati
            condition.DataBar.Color = Color.Orange;
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            condition.DataBar.ShowValue = false;

            // Imposta le proprietà del bordo
            condition.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            condition.DataBar.BarBorder.Color = Color.Plum;

            // Imposta il tipo di riempimento
            condition.DataBar.BarFillType = DataBarFillType.Gradient;

            // Imposta le proprietà dell'asse
            condition.DataBar.AxisColor = Color.Red;
            condition.DataBar.AxisPosition = DataBarAxisPosition.Automatic;

            // Configura il formato della barra negativa
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Salva la cartella di lavoro
            workbook.Save("DataBarNegativeFormatDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [NegativeBarFormat](../../negativebarformat/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


