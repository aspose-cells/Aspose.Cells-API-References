---
title: "Range.UnMerge"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Separa le celle unite di questo intervallo"
type: docs
url: /it/net/aspose.cells/range/unmerge/
---
## Range.UnMerge method

Separa le celle unite di questo intervallo.

```csharp
public void UnMerge()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Unisci le celle da B2 a D4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "D4");
            range.Merge();
            
            // Verifica se la cella B2 è unita prima di separarla
            Console.WriteLine("Before UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
            
            // Separa l'intervallo
            range.UnMerge();
            
            // Verifica se la cella B2 è unita dopo averla separata
            Console.WriteLine("After UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


