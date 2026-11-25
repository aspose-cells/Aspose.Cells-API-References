---
title: "Enum TargetModeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.TargetModeType enum. Rappresenta il tipo di modalità di destinazione"
type: docs
url: /it/net/aspose.cells/targetmodetype/
---
## TargetModeType enumeration

Rappresenta il tipo di modalità di destinazione.

```csharp
public enum TargetModeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| External | `0` | Link esterno |
| FilePath | `1` | Percorsi locali e completi a file o cartelle. |
| Email | `2` | Email. |
| CellReference | `3` | Collegamento su cella o intervallo denominato. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTargetModeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un collegamento ipertestuale esterno
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Ottieni il collegamento ipertestuale e verifica il suo TargetModeType
            Hyperlink link = worksheet.Hyperlinks[0];
            Console.WriteLine("Hyperlink TargetModeType: " + link.LinkType);
            
            // Elimina il collegamento ipertestuale
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


