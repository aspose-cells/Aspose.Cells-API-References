---
title: "BuiltInDocumentPropertyCollection.LinksUpToDate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection property. Gibt an, ob Hyperlinks in einem Dokument aktuell sind"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/linksuptodate/
---
## BuiltInDocumentPropertyCollection.LinksUpToDate property

Gibt an, ob Hyperlinks in einem Dokument aktuell sind.

```csharp
public bool LinksUpToDate { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLinksUpToDateDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf die integrierte Sammlung von Dokumenteigenschaften
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Setzen Sie die LinksUpToDate-Eigenschaft, um anzugeben, ob Hyperlinks aktuell sind
            builtInProperties.LinksUpToDate = true;

            // Fügen Sie einen einfachen Hyperlink hinzu, um die Eigenschaft zu demonstrieren
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Speichere die Arbeitsmappe
            workbook.Save("LinksUpToDateDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


