---
title: "BuiltInDocumentPropertyCollection.Keywords"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Gibt die Schlüsselwörter des Dokuments zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/keywords/
---
## BuiltInDocumentPropertyCollection.Keywords property

Liest oder setzt die Dokument‑Stichwörter.

```csharp
public string Keywords { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyKeywordsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Die Schlüsselwörter-Eigenschaft festlegen
            workbook.BuiltInDocumentProperties.Keywords = "Sample Keywords, Aspose.Cells, Demo";
            
            // Speichere die Arbeitsmappe
            workbook.Save("output_keywords.xlsx");
            
            // Laden Sie die gespeicherte Arbeitsmappe, um die Schlüsselwörter-Eigenschaft zu überprüfen
            Workbook loadedWorkbook = new Workbook("output_keywords.xlsx");
            
            // Die Schlüsselwörter-Eigenschaft anzeigen
            Console.WriteLine("Document Keywords: " + loadedWorkbook.BuiltInDocumentProperties.Keywords);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


