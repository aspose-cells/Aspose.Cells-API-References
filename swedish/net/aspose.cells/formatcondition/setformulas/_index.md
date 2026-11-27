---
title: "FormatCondition.SetFormulas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-metod. Anger värdet eller uttrycket som är kopplat till detta formatvillkor"
type: docs
url: /sv/net/aspose.cells/formatcondition/setformulas/
---
## FormatCondition.SetFormulas method

Anger värdet eller uttrycket som är kopplat till detta formatvillkor.

```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula1 | String | Värdet eller uttrycket som är kopplat till detta formatvillkor. Om inmatningsvärdet börjar med '=', tas det som en formel. Annars tas det som ett vanligt värde (text, nummer, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\"=...\"". |
| formula2 | String | Värdet eller uttrycket som är kopplat till detta formatvillkor. Indataformatet är samma som formula1. |
| isR1C1 | Boolean | Om formeln är en R1C1-formel. |
| isLocal | Boolean | Om formeln är lokalt formaterad. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodSetFormulasWithStringStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int formatIndex = cfs.Add();
            FormatConditionCollection fcs = cfs[formatIndex];
            
            fcs.AddArea(CellArea.CreateCellArea("A1", "C10"));
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcs[conditionIndex];
            
            fc.Operator = OperatorType.Between;
            fc.SetFormulas("=1", "=2", false, false);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


