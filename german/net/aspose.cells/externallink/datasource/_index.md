---
title: "ExternalLink.DataSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLink-Eigenschaft. Stellt die Datenquelle des externen Links dar"
type: docs
url: /de/net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

Repräsentiert die Datenquelle des externen Links.

```csharp
public string DataSource { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyDataSourceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsblatt hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen externen Link zu einer anderen Arbeitsmappe
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Lade die gespeicherte Arbeitsmappe, um externe Links zu prüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Greife auf die DataSource-Eigenschaft des externen Links zu
            if (loadedWorkbook.Worksheets.ExternalLinks.Count > 0)
            {
                string dataSource = loadedWorkbook.Worksheets.ExternalLinks[0].DataSource;
                Console.WriteLine("External link data source: " + dataSource);
            }
        }
    }
}
```

### Siehe auch

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


