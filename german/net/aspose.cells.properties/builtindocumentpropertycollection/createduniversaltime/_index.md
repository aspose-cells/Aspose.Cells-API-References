---
title: "BuiltInDocumentPropertyCollection.CreatedUniversalTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection property. Liest oder setzt die universelle Zeit der Dokumenterstellung"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/createduniversaltime/
---
## BuiltInDocumentPropertyCollection.CreatedUniversalTime property

Liest oder setzt die universelle Zeit der Dokumenterstellung.

```csharp
public DateTime CreatedUniversalTime { get; set; }
```

### Hinweise

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedUniversalTimeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze die CreatedUniversalTime-Eigenschaft
            DateTime creationTime = new DateTime(2023, 5, 15, 15, 30, 0, DateTimeKind.Utc);
            workbook.BuiltInDocumentProperties.CreatedUniversalTime = creationTime;
            
            // Zeige die CreatedUniversalTime-Eigenschaft an
            Console.WriteLine("Document created (UTC): " + 
                workbook.BuiltInDocumentProperties.CreatedUniversalTime.ToString());
            
            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


