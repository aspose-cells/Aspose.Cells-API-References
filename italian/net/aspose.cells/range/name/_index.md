---
title: "Range.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Restituisce o imposta il nome dell'intervallo"
type: docs
url: /it/net/aspose.cells/range/name/
---
## Range.Name property

Ottiene o imposta il nome dell'intervallo.

```csharp
public string Name { get; set; }
```

### Osservazioni

Gli intervalli denominati sono supportati. Ad esempio,

range.Name = "Sheet1!MyRange";

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo (colonne A a B)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, true);
            
            // Imposta la proprietà Name per l'intervallo
            range.Name = "testRange";
            
            // Verifica che il nome sia stato impostato
            Console.WriteLine("Range name: " + range.Name);
            
            // Salva la cartella di lavoro
            workbook.Save("RangeWithName.xlsx");
            
            // Apri il file salvato per dimostrare che il nome persiste
            Workbook loadedWorkbook = new Workbook("RangeWithName.xlsx");
            Aspose.Cells.Range loadedRange = loadedWorkbook.Worksheets[0].Cells.CreateRange(0, 2, true);
            Console.WriteLine("Loaded range name: " + loadedRange.Name);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


