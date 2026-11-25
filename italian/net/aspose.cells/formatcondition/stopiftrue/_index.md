---
title: "FormatCondition.StopIfTrue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "FormatCondition property. True nessuna regola con priorità inferiore può essere applicata su questa regola quando questa regola restituisce true. Si applica solo a Excel 2007"
type: docs
url: /it/net/aspose.cells/formatcondition/stopiftrue/
---
## FormatCondition.StopIfTrue property

True, nessuna regola con priorità inferiore può essere applicata sopra questa regola, quando questa regola restituisce true. Valida solo per Excel 2007;

```csharp
public bool StopIfTrue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStopIfTrueDemo
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

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Aggiungi condizione e imposta StopIfTrue
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            FormatCondition condition = fcs[conditionIndex];
            condition.StopIfTrue = true;
            
            // Aggiungi un'altra condizione che normalmente sovrascriverebbe la prima
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "25", "");
            FormatCondition condition2 = fcs[conditionIndex2];
            condition2.StopIfTrue = false;

            // Salva la cartella di lavoro
            workbook.Save("StopIfTrueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


