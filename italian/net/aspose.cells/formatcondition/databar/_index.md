---
title: "FormatCondition.DataBar"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottieni l'istanza DataBar della formattazione condizionale. Il colore predefinito dell'istanza è blu. Valida solo per il tipo DataBar"
type: docs
url: /it/net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

Ottieni l'istanza "DataBar" della formattazione condizionale. Il colore dell'istanza predefinita è blu. Valida solo per type = DataBar.

```csharp
public DataBar DataBar { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyDataBarDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Aggiungi formattazione condizionale della barra dati
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Imposta l'intervallo per la formattazione condizionale
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Aggiungi la condizione barra dati e imposta le proprietà
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcs[conditionIndex];
            
            // Configura le proprietà DataBar
            DataBar dataBar = condition.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            dataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            dataBar.Color = System.Drawing.Color.Green;

            // Salva la cartella di lavoro
            workbook.Save("DataBarExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


