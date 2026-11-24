---
title: "BuiltInDocumentPropertyCollection.Title"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Liest oder setzt den Titel des Dokuments"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/title/
---
## BuiltInDocumentPropertyCollection.Title property

Liest oder setzt den Titel des Dokuments.

```csharp
public string Title { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTitleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze die Title-Eigenschaft
            workbook.BuiltInDocumentProperties.Title = "Sample Document Title";
            
            // Zeige die Title-Eigenschaft
            Console.WriteLine("Document Title: " + workbook.BuiltInDocumentProperties.Title);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


