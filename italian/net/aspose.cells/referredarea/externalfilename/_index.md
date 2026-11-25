---
title: "ReferredArea.ExternalFileName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReferredArea. Ottieni il nome del file esterno se questo è un riferimento esterno"
type: docs
url: /it/net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

Ottieni il nome del file esterno se si tratta di un riferimento esterno.

```csharp
public string ExternalFileName { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyExternalFileNameDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con riferimento esterno
            Workbook wb = new Workbook();
            
            // Crea un nome che fa riferimento a una cartella di lavoro esterna
            int index = wb.Worksheets.Names.Add("RefExternalName");
            wb.Worksheets.Names[index].RefersTo = "='[ExternalLinkSource.xlsx]Sheet1'!$A$1:$C$3";
            
            // Ottieni l'area di riferimento
            ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
            
            // Dimostra la proprietà ExternalFileName
            Console.WriteLine("External File Name: " + ra.ExternalFileName);
            Console.WriteLine("Sheet Name: " + ra.SheetName);
            Console.WriteLine("Area: R" + ra.StartRow + "C" + ra.StartColumn + 
                              " to R" + ra.EndRow + "C" + ra.EndColumn);
            
            // Verifica il nome del file esterno
            if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
            {
                Console.WriteLine("Error: ExternalFileName should be ExternalLinkSource.xlsx");
            }
        }
    }
}
```

### Vedi anche

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


