---
title: "ExternalLink.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLink-Eigenschaft. Gibt den Typ des externen Links zurück"
type: docs
url: /de/net/aspose.cells/externallink/type/
---
## ExternalLink.Type property

Ermittelt den Typ des externen Links.

```csharp
public ExternalLinkType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsblatt hinzufügen
            Worksheet sheet = workbook.Worksheets[0];
            
            // Erstelle einen externen Link zu einer anderen Arbeitsmappe
            sheet.Cells["A1"].Formula = "='[link.xls]Sheet1'!A1";
            
            // Hole den externen Link
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Anzeige des Typs des externen Links
            Console.WriteLine("External Link Type: " + externalLink.Type);
            
            // Ändere die Datenquelle des externen Links
            externalLink.DataSource = "d:\\link.xls";
            
            // Speichere die Arbeitsmappe
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


