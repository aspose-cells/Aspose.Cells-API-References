---
title: "DataBar.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Ottieni o imposta il colore di questa DataBar"
type: docs
url: /it/net/aspose.cells/databar/color/
---
## DataBar.Color property

Ottieni o imposta il colore di questa DataBar.

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
    public class DataBarPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo di celle
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["E3"].PutValue(10);
            worksheet.Cells["F3"].PutValue(20);
            worksheet.Cells["G3"].PutValue(30);
            worksheet.Cells["E4"].PutValue(15);
            worksheet.Cells["F4"].PutValue(25);
            worksheet.Cells["G4"].PutValue(35);

            // Aggiungi formattazione condizionale con barra dei dati
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Imposta le proprietà della barra dei dati includendo il colore
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

            // Imposta le proprietà della barra negativa
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Applica la formattazione all'intervallo
            conditions.AddArea(area);

            // Salva la cartella di lavoro
            workbook.Save("DataBarPropertyColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBarPropertyColorDemo executed successfully.");
        }
    }
}
```

### Vedi anche

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


