---
title: "CellsHelper.SignificantDigits"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsHelper. Ottiene e imposta il numero di cifre significative. Il valore predefinito è 17"
type: docs
url: /it/net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Ottiene e imposta il numero di cifre significative. Il valore predefinito è 17.

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static int SignificantDigits { get; set; }
```

### Osservazioni

Può essere solo 15 o 17 ora. NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare [`SignificantDigitsType`](../significantdigitstype/). Questa proprietà verrà rimossa 12 mesi dopo, a partire da giugno 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Imposta le cifre significative
            CellsHelper.SignificantDigits = 15;
            
            // Dimostra l'uso della proprietà
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            
            // Crea una cartella di lavoro per dimostrare le cifre significative nei calcoli
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta valori che saranno influenzati dalle cifre significative
            worksheet.Cells["A1"].PutValue(1.2345678912345678);
            worksheet.Cells["A2"].PutValue(1.2345678912345678);
            worksheet.Cells["A3"].Formula = "=A1+A2";
            
            // Calcola le formule con le cifre significative impostate
            workbook.CalculateFormula();
            
            // Restituisci i risultati
            Console.WriteLine("Value with significant digits: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


