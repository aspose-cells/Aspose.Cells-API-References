---
title: "UnionRange.Merge"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo UnionRange. Combina un intervallo di celle in una singola cella"
type: docs
url: /it/net/aspose.cells/unionrange/merge/
---
## UnionRange.Merge method

Combina un intervallo di celle in una singola cella.

```csharp
public void Merge()
```

### Osservazioni

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra nell'intervallo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodMergeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo di celle (A1:B2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            
            // Inserisci alcuni dati nelle celle per visualizzare l'unione
            range[0, 0].PutValue("Before Merge");
            range[0, 1].PutValue("A1");
            range[1, 0].PutValue("B1");
            range[1, 1].PutValue("B2");
            
            try
            {
                // Crea un UnionRange dall'Intervallo
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
                
                // Chiama il metodo Merge
                unionRange.Merge();
                
                // Inserisci il valore nella cella unita
                unionRange.PutValue("Merged A1:B2", true, true);
                
                Console.WriteLine("Cells merged successfully");
                
                // Decommenta per vedere l'effetto della separazione
                // unionRange.UnMerge();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Merge method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("MethodMergeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


