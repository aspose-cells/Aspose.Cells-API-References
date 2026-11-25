---
title: "DataBar.MinCfvo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Ottieni o imposta questo oggetto valore minimo di DataBar. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Max"
type: docs
url: /it/net/aspose.cells/databar/mincfvo/
---
## DataBar.MinCfvo property

Ottieni o imposta l'oggetto valore minimo di questa DataBar. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Max.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinCfvoDemo
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

            // Ottieni la raccolta di formattazione condizionale
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];

            // Crea una barra dati con MinCfvo impostato al tipo "Value"
            fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[0].DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MinCfvo.Value = "5"; // Minimum value for the data bar

            // Imposta l'intervallo della barra dati
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Salva la cartella di lavoro
            workbook.Save("DataBarMinCfvoDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


