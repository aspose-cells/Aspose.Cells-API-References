---
title: "CopyOptions.CopyNames"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CopyOptions. Indica se copiare i nomi"
type: docs
url: /it/net/aspose.cells/copyoptions/copynames/
---
## CopyOptions.CopyNames property

Indica se copiare i nomi.

```csharp
public bool CopyNames { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyNamesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di origine con intervalli denominati
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Crea un intervallo denominato nella cartella di lavoro di origine
            sourceSheet.Cells["A1"].PutValue("Test Value");
            int index = sourceWorkbook.Worksheets.Names.Add("SourceName");
            sourceWorkbook.Worksheets.Names[index].RefersTo = "=Sheet1!$A$1";

            // Crea una cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            
            // Copia il foglio di lavoro con CopyNames=true
            destWorkbook.Worksheets[0].Copy(sourceSheet, new CopyOptions { CopyNames = true });

            // Verifica che l'intervallo denominato sia stato copiato
            Name copiedName = destWorkbook.Worksheets.Names["SourceName"];
            if (copiedName != null)
            {
                Console.WriteLine("Named range copied successfully: " + copiedName.RefersTo);
            }
            else
            {
                Console.WriteLine("Named range was not copied");
            }
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


