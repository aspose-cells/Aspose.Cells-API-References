---
title: "WorksheetCollection.CustomDocumentProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Gibt eine DocumentProperty-Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt"
type: docs
url: /de/net/aspose.cells/worksheetcollection/customdocumentproperties/
---
## WorksheetCollection.CustomDocumentProperties property

Gibt eine [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/)‑Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Benutzerdefinierte Dokumenteigenschaften hinzufügen
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("CreatedDate", DateTime.Now);
            workbook.Worksheets.CustomDocumentProperties.Add("Version", 1.2);
            
            // Greife auf die Eigenschaften zu und zeige sie an
            Console.WriteLine("Author: " + workbook.Worksheets.CustomDocumentProperties["Author"]);
            Console.WriteLine("Created: " + workbook.Worksheets.CustomDocumentProperties["CreatedDate"]);
            Console.WriteLine("Version: " + workbook.Worksheets.CustomDocumentProperties["Version"]);
        }
    }
}
```

### Siehe auch

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


