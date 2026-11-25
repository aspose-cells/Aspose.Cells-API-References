---
title: "DataBar.MaxCfvo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Ottieni o imposta questo oggetto valore massimo della barra dati. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Min su di esso"
type: docs
url: /it/net/aspose.cells/databar/maxcfvo/
---
## DataBar.MaxCfvo property

Ottieni o imposta l'oggetto valore massimo di questa DataBar. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Min.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxCfvoDemo
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

            // Aggiungi formattazione condizionale della barra dati
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Aggiungi barra dati
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;

            // Imposta valore MaxCfvo
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            dataBar.MaxCfvo.Value = 50;

            // Salva la cartella di lavoro
            workbook.Save("DataBarMaxCfvoDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


