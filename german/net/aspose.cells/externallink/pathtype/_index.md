---
title: "ExternalLink.PathType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLink-Eigenschaft. Gibt den Pfadtyp dieses externen Links zurück"
type: docs
url: /de/net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

Erhalte den Pfadtyp dieses externen Links

```csharp
public string PathType { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyPathTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsblatt hinzufügen
            Worksheet sheet = workbook.Worksheets[0];
            
            // Erstelle einen externen Link zu einer anderen Arbeitsmappe
            sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
            
            // Hole den externen Link
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Zeigt den Pfadtyp des externen Links an
            Console.WriteLine("Path Type: " + externalLink.PathType);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ExternalLinkDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


