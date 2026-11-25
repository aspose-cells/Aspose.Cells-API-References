---
title: "CellsHelper.ConvertR1C1FormulaToA1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Converte la formula r1c1 della cella nella formula A1"
type: docs
url: /it/net/aspose.cells/cellshelper/convertr1c1formulatoa1/
---
## CellsHelper.ConvertR1C1FormulaToA1 method

Converte la formula r1c1 della cella nella formula A1.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertR1C1FormulaToA1(string r1c1Formula, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| r1c1Formula | String | La formula r1c1. |
| riga | Int32 | L'indice di riga della cella. |
| colonna | Int32 | L'indice di colonna della cella. |

### Valore di ritorno

La formula A1.

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Worksheet.ConvertFormulaReferenceStyle(). Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertR1C1FormulaToA1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta le formule R1C1 nelle celle
            worksheet.Cells["A1"].R1C1Formula = "=R[1]C";
            worksheet.Cells["B1"].R1C1Formula = "=RC[1]";
            worksheet.Cells["A2"].R1C1Formula = "=R2C3";
            worksheet.Cells["B2"].R1C1Formula = "=R[-1]C[-1]";

            // Converti le formule R1C1 nello stile A1
            string a1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A1"].R1C1Formula, 0, 0);
            string b1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B1"].R1C1Formula, 0, 0);
            string a2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A2"].R1C1Formula, 1, 2);
            string b2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B2"].R1C1Formula, 1, 1);

            // Restituisci i risultati
            Console.WriteLine("A1 R1C1: {0} -> A1: {1}", worksheet.Cells["A1"].R1C1Formula, a1Converted);
            Console.WriteLine("B1 R1C1: {0} -> A1: {1}", worksheet.Cells["B1"].R1C1Formula, b1Converted);
            Console.WriteLine("A2 R1C1: {0} -> A1: {1}", worksheet.Cells["A2"].R1C1Formula, a2Converted);
            Console.WriteLine("B2 R1C1: {0} -> A1: {1}", worksheet.Cells["B2"].R1C1Formula, b2Converted);
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


