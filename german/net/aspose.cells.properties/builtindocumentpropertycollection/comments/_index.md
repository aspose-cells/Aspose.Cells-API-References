---
title: "BuiltInDocumentPropertyCollection.Comments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Ruft die Dokumentkommentare ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/comments/
---
## BuiltInDocumentPropertyCollection.Comments property

Liest oder setzt die Dokumentkommentare.

```csharp
public string Comments { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCommentsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf integrierte Dokumenteigenschaften
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Die Comments-Eigenschaft festlegen
            properties.Comments = "This is a sample comment for demonstration.";
            
            // Die Comments-Eigenschaft anzeigen
            Console.WriteLine("Document Comments: " + properties.Comments);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


