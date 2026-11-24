---
title: "BuiltInDocumentPropertyCollection.CreatedTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection property. Gibt das Erstellungsdatum des Dokuments in der lokalen Zeitzone zurück oder legt es fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/createdtime/
---
## BuiltInDocumentPropertyCollection.CreatedTime property

Liest oder setzt das Erstellungsdatum des Dokuments in der lokalen Zeitzone.

```csharp
public DateTime CreatedTime { get; set; }
```

### Hinweise

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze die CreatedTime-Eigenschaft auf die aktuelle Zeit
            DateTime currentTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.CreatedTime = currentTime;
            
            // Speichere die Arbeitsmappe
            string outputPath = "output_CreatedTimeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Laden Sie die gespeicherte Arbeitsmappe, um die Eigenschaft zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            DateTime loadedTime = loadedWorkbook.BuiltInDocumentProperties.CreatedTime;
            
            Console.WriteLine("Original CreatedTime: " + currentTime);
            Console.WriteLine("Loaded CreatedTime: " + loadedTime);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


