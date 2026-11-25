---
title: "ExternalLink.PathType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExternalLink property. Ottieni il tipo di percorso di questo collegamento esterno"
type: docs
url: /it/net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

Ottieni il tipo di percorso di questo collegamento esterno

```csharp
public string PathType { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyPathTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crea un collegamento esterno a un altro foglio di lavoro
            sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
            
            // Ottieni il collegamento esterno
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Visualizza il tipo di percorso del collegamento esterno
            Console.WriteLine("Path Type: " + externalLink.PathType);
            
            // Salva la cartella di lavoro
            workbook.Save("ExternalLinkDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


