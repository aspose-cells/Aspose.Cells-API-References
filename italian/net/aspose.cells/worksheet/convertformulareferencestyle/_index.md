---
title: "Worksheet.ConvertFormulaReferenceStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Converte lo stile di riferimento della formula"
type: docs
url: /it/net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

Converte lo stile di riferimento della formula.

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | La formula da convertire. |
| toR1C1 | Booleano | Quale stile di riferimento utilizzare per convertire la formula. Se la formula originale è nello stile di riferimento A1, questo valore dovrebbe essere true affinché la formula venga convertita dallo stile A1 allo stile R1C1; se la formula originale è nello stile di riferimento R1C1, questo valore dovrebbe essere false affinché la formula venga convertita dallo stile R1C1 allo stile A1; |
| baseCellRow | Int32 | L'indice di riga della cella di base. |
| baseCellColumn | Int32 | L'indice di colonna della cella di base. |

### Valore di ritorno

La formula convertita.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Esempio 1: Converti lo stile R1C1 in stile A1
            string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
            string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
            Console.WriteLine("Converted formula: " + formulaA1);

            // Esempio 2: Converti con riferimenti misti
            string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
            string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
            Console.WriteLine("Converted mixed formula: " + convertedMixed);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


