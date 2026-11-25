---
title: "CellsHelper.ConvertA1FormulaToR1C1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Converte la formula A1 della cella nella formula r1c1"
type: docs
url: /it/net/aspose.cells/cellshelper/converta1formulator1c1/
---
## CellsHelper.ConvertA1FormulaToR1C1 method

Converte la formula A1 della cella nella formula r1c1.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | La formula A1. |
| riga | Int32 | L'indice di riga della cella. |
| colonna | Int32 | L'indice di colonna della cella. |

### Valore di ritorno

La formula R1C1.

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Worksheet.ConvertFormulaReferenceStyle(). Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertA1FormulaToR1C1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Converti la formula in stile A1 in stile R1C1
            string r1c1Formula = CellsHelper.ConvertA1FormulaToR1C1("=A1+B2", 0, 0);
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


