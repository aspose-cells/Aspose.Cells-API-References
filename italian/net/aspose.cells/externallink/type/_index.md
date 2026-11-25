---
title: "ExternalLink.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExternalLink property. Ottiene il tipo di collegamento esterno"
type: docs
url: /it/net/aspose.cells/externallink/type/
---
## ExternalLink.Type property

Ottiene il tipo di collegamento esterno.

```csharp
public ExternalLinkType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crea un collegamento esterno a un altro foglio di lavoro
            sheet.Cells["A1"].Formula = "='[link.xls]Sheet1'!A1";
            
            // Ottieni il collegamento esterno
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Visualizza il tipo di collegamento esterno
            Console.WriteLine("External Link Type: " + externalLink.Type);
            
            // Modifica la fonte dati del collegamento esterno
            externalLink.DataSource = "d:\\link.xls";
            
            // Salva la cartella di lavoro
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


