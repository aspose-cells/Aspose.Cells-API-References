---
title: "UnionRange.UnMerge"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo UnionRange. Separa le celle unite di questo intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/unmerge/
---
## UnionRange.UnMerge method

Separa le celle unite di questo intervallo.

```csharp
public void UnMerge()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo e unisci le celle
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
            
            // Unisci le celle e inserisci un valore
            unionRange.Merge();
            unionRange.PutValue("Merged Cells", true, true);
            
            try
            {
                // Chiama il metodo UnMerge
                unionRange.UnMerge();
                
                Console.WriteLine("Cells unmerged successfully");
                
                // Inserisci valori nelle celle separate per dimostrare l'effetto
                worksheet.Cells["A1"].PutValue("A1");
                worksheet.Cells["A2"].PutValue("A2");
                worksheet.Cells["B1"].PutValue("B1");
                worksheet.Cells["B2"].PutValue("B2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnMerge method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("MethodUnMergeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


