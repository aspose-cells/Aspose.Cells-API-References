---
title: "FormatCondition.SetFormulas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "FormatCondition method. Imposta il valore o l'espressione associata a questa condizione di formattazione"
type: docs
url: /it/net/aspose.cells/formatcondition/setformulas/
---
## FormatCondition.SetFormulas method

Imposta il valore o l'espressione associati a questa condizione di formato.

```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula1 | String | Il valore o l'espressione associata a questa condizione di formattazione. Se il valore di input inizia con '=', verrà considerato una formula. Altrimenti verrà considerato un valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirlo come formula nel formato: "=\"=...\"". |
| formula2 | String | Il valore o l'espressione associati a questa condizione di formattazione. Il formato di input è lo stesso di formula1 |
| isR1C1 | Booleano | Indica se la formula è una formula R1C1. |
| isLocal | Booleano | Se la formula è formattata secondo la locale. |

### Esempi

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

### Vedi anche

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


