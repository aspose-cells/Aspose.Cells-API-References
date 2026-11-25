---
title: "Range.Union"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Restituisce l'unione di due intervalli"
type: docs
url: /it/net/aspose.cells/range/union/
---
## Range.Union method

Restituisce l'unione di due intervalli.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList Union(Range range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Intervallo | L'intervallo |

### Valore di ritorno

L'unione di due intervalli.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Range.UnionRanges(). Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due intervalli per dimostrare Union
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:C3");

            // Inserisci alcuni dati negli intervalli
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");

            try
            {
                // Chiama il metodo Union (nota: questa è la versione obsoleta)
                ArrayList unionResult = range1.Union(range2);

                Console.WriteLine("Union method executed successfully");
                Console.WriteLine($"Number of ranges in union: {unionResult.Count}");

                // Visualizza gli indirizzi di tutti gli intervalli nell'unione
                foreach (Aspose.Cells.Range r in unionResult)
                {
                    Console.WriteLine($"Union range address: {r.Address}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("RangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


