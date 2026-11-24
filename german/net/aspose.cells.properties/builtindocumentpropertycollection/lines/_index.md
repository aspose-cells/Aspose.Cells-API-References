---
title: "BuiltInDocumentPropertyCollection.Lines"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection property. Stellt eine Schätzung der Anzahl von Zeilen im Dokument dar"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/lines/
---
## BuiltInDocumentPropertyCollection.Lines property

Stellt eine Schätzung der Anzahl von Zeilen im Dokument dar.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```

### Hinweise

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf integrierte Dokumenteigenschaften
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Zeige den aktuellen Lines-Wert an (Schätzung der Zeilenanzahl im Dokument)
            Console.WriteLine("Current Lines value: " + properties.Lines);
            
            // Setze einen neuen Wert für die Lines-Eigenschaft
            properties.Lines = 150;
            
            // Füge etwas Inhalt hinzu, um den Zweck der Eigenschaft zu demonstrieren
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Line " + (i + 1);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PropertyLinesDemo.xlsx");
            
            // Hinweis: Die Lines-Eigenschaft ist eine Schätzung und wird nicht automatisch mit dem tatsächlichen Inhalt aktualisiert
            // Sie wird hauptsächlich für Dokument-Metadatenzwecke verwendet
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


