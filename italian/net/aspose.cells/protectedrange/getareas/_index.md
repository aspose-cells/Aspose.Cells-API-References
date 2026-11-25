---
title: "ProtectedRange.GetAreas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ProtectedRange. Ottiene tutte le aree riferite"
type: docs
url: /it/net/aspose.cells/protectedrange/getareas/
---
## ProtectedRange.GetAreas method

Ottiene tutte le aree di riferimento.

```csharp
public CellArea[] GetAreas()
```

### Valore di ritorno

Restituisce tutte le aree riferite.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeMethodGetAreasDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la collezione di intervalli protetti
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Aggiungi un intervallo protetto
            int index = protectedRanges.Add("TestRange", 0, 0, 10, 10);
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Ottieni le aree dell'intervallo protetto
            CellArea[] areas = protectedRange.GetAreas();
            
            // Stampa il numero di aree (dovrebbe essere 1 per questo intervallo semplice)
            Console.WriteLine("Number of areas in protected range: " + areas.Length);
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectedRangeExample.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


