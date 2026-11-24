---
title: "BuiltInDocumentPropertyCollection.Paragraphs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Stellt eine Schätzung der Anzahl der Absätze im Dokument dar"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/paragraphs/
---
## BuiltInDocumentPropertyCollection.Paragraphs property

Stellt eine Schätzung der Anzahl der Absätze im Dokument dar.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Paragraphs { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyParagraphsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf integrierte Dokumenteigenschaften
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Zeige den aktuellen Paragraphs-Wert (veraltete Eigenschaft)
            Console.WriteLine("Current Paragraphs value: " + properties.Paragraphs);

            // Setze einen neuen Wert für Paragraphs (veraltete Eigenschaft)
            properties.Paragraphs = 15;
            Console.WriteLine("Updated Paragraphs value: " + properties.Paragraphs);

            // Einige Inhalte hinzufügen, um die Wirkung der Eigenschaft zu demonstrieren
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is paragraph 1");
            worksheet.Cells["A2"].PutValue("This is paragraph 2");
            worksheet.Cells["A3"].PutValue("This is paragraph 3");

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyParagraphsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


