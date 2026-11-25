---
title: "Cells.GetMergedAreas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene tutte le celle unite"
type: docs
url: /it/net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Restituisce tutte le celle unite.

```csharp
public CellArea[] GetMergedAreas()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMergedAreasDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea alcune celle unite
            worksheet.Cells.Merge(0, 0, 2, 2); // Merge A1:B2
            worksheet.Cells.Merge(3, 3, 3, 2); // Merge D4:E4
            worksheet.Cells.Merge(5, 0, 1, 5); // Merge A6:E6
            
            // Ottieni tutte le aree unite
            CellArea[] mergedAreas = worksheet.Cells.GetMergedAreas();
            
            // Visualizza le informazioni sulle aree unite
            Console.WriteLine("Number of merged areas: " + mergedAreas.Length);
            foreach (CellArea area in mergedAreas)
            {
                Console.WriteLine($"Merged area: StartRow={area.StartRow}, StartColumn={area.StartColumn}, " +
                    $"EndRow={area.EndRow}, EndColumn={area.EndColumn}");
            }
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


