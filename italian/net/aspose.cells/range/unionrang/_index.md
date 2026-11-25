---
title: "Range.UnionRang"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Restituisce il risultato dell'unione di due intervalli"
type: docs
url: /it/net/aspose.cells/range/unionrang/
---
## Range.UnionRang method

Restituisce il risultato dell'unione di due intervalli.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Intervallo | L'intervallo |

### Valore di ritorno

L'unione di due intervalli.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, usa il metodo Range.UnionRanges(). Questo metodo sarà rimosso 12 mesi dopo da maggio 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity

    public class RangeMethodUnionRangWithRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due intervalli per dimostrare UnionRang
            Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Range range2 = worksheet.Cells.CreateRange("C3:D4");

            // Imposta alcuni valori negli intervalli per visualizzazione
            range1[0, 0].PutValue("Range1");
            range1[1, 1].PutValue("Data");
            range2[0, 0].PutValue("Range2");
            range2[1, 1].PutValue("Data");

            try
            {
                // Chiama il metodo UnionRang per combinare i due intervalli
                Range[] unionResult = range1.UnionRang(range2);

                // Visualizza informazioni sul risultato dell'unione
                Console.WriteLine("UnionRang method executed successfully.");
                Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
                Console.WriteLine($"First union range address: {unionResult[0].Address}");
                Console.WriteLine($"Second union range address: {unionResult[1].Address}");

                // Segna gli intervalli di unione con un bordo per visualizzazione
                foreach (Range r in unionResult)
                {
                    r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


