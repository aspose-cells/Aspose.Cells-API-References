---
title: "ExternalLink.DataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExternalLink property. Rappresenta la fonte dati del collegamento esterno"
type: docs
url: /it/net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

Rappresenta la fonte dati del collegamento esterno.

```csharp
public string DataSource { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyDataSourceDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un collegamento esterno a un altro foglio di lavoro
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Carica il foglio di lavoro salvato per verificare i collegamenti esterni
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Accedi alla proprietà DataSource del collegamento esterno
            if (loadedWorkbook.Worksheets.ExternalLinks.Count > 0)
            {
                string dataSource = loadedWorkbook.Worksheets.ExternalLinks[0].DataSource;
                Console.WriteLine("External link data source: " + dataSource);
            }
        }
    }
}
```

### Vedi anche

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


