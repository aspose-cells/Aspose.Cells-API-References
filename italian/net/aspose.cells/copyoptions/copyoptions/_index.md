---
title: "CopyOptions.CopyOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore CopyOptions. Costruttore CopyOptions"
type: docs
url: /it/net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

Costruttore CopyOptions.

```csharp
public CopyOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e ottieni il primo foglio di lavoro
            Worksheet sourceSheet = workbook.Worksheets[0];
            Worksheet destSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            
            // Aggiungi dati di esempio al foglio di origine
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            sourceSheet.Cells["A4"].PutValue(300);
            
            // Crea CopyOptions usando il costruttore
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;
            
            // Copia le righe con le opzioni
            destSheet.Cells.CopyRows(sourceSheet.Cells, 0, 0, sourceSheet.Cells.MaxDisplayRange.RowCount, options);
            
            // Salva la cartella di lavoro
            workbook.Save("CopyOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


