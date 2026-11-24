---
title: "BuiltInDocumentPropertyCollection.ContentStatus"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Liest oder setzt den Inhaltsstatus des Dokuments"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/contentstatus/
---
## BuiltInDocumentPropertyCollection.ContentStatus property

Liest oder setzt den Inhaltsstatus des Dokuments.

```csharp
public string ContentStatus { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentStatusDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Setze integrierte Dokumenteigenschaften einschließlich ContentStatus
            workbook.BuiltInDocumentProperties.ContentStatus = "Draft";
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";

            // Speichere die Arbeitsmappe
            workbook.Save("DocumentWithContentStatus.xlsx", SaveFormat.Xlsx);

            // Laden der gespeicherten Arbeitsmappe, um Eigenschaften zu überprüfen
            Workbook loadedWorkbook = new Workbook("DocumentWithContentStatus.xlsx");
            
            // Zeige die ContentStatus-Eigenschaft
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


