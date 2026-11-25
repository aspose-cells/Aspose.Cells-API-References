---
title: "Range.Transpose"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Trasponi ruota i dati da righe a colonne o viceversa"
type: docs
url: /it/net/aspose.cells/range/transpose/
---
## Range.Transpose method

Trasponi (ruota) i dati dalle righe alle colonne o viceversa.

```csharp
public void Transpose()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodTransposeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Riempie dati di esempio in un intervallo 3x3 (A1:C3)
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].PutValue(6);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["C3"].PutValue(9);
            
            // Crea un intervallo (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            
            // Trasponi l'intervallo
            range.Transpose();
            
            // Salva la cartella di lavoro
            workbook.Save("TransposedOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


