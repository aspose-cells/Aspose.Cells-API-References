---
title: "BuiltInDocumentPropertyCollection.LastSavedBy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection property. Gibt den Namen des letzten Autors zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedby/
---
## BuiltInDocumentPropertyCollection.LastSavedBy property

Liest oder setzt den Namen des letzten Autors.

```csharp
public string LastSavedBy { get; set; }
```

### Hinweise

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedByDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze integrierte Dokumenteigenschaften einschließlich LastSavedBy
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";
            workbook.BuiltInDocumentProperties.LastSavedBy = "Jane Smith";
            
            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
            
            // Laden der gespeicherten Arbeitsmappe, um Eigenschaften zu überprüfen
            Workbook loadedWorkbook = new Workbook("DocumentPropertiesDemo.xlsx");
            
            // Gib die LastSavedBy-Eigenschaft aus
            Console.WriteLine("Last saved by: " + loadedWorkbook.BuiltInDocumentProperties.LastSavedBy);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


