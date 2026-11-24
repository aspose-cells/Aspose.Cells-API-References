---
title: "BuiltInDocumentPropertyCollection.Category"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Ruft die Kategorie des Dokuments ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/category/
---
## BuiltInDocumentPropertyCollection.Category property

Liest oder setzt die Kategorie des Dokuments.

```csharp
public string Category { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCategoryDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            var workbook = new Workbook();
            
            // Integrierte Dokumenteigenschaften festlegen
            workbook.BuiltInDocumentProperties.Category = "Financial Report";
            workbook.BuiltInDocumentProperties.ContentStatus = "Final";
            
            // In den Speicherstream speichern
            var stream = new MemoryStream();
            workbook.Save(stream, SaveFormat.Xlsx);
            
            // Laden Sie die Arbeitsmappe aus dem Stream zurück
            stream.Position = 0;
            var loadedWorkbook = new Workbook(stream);
            
            // Zeigen Sie die Eigenschaften an
            Console.WriteLine("Category: " + loadedWorkbook.BuiltInDocumentProperties.Category);
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


