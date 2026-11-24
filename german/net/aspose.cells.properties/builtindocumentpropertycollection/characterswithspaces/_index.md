---
title: "BuiltInDocumentPropertyCollection.CharactersWithSpaces"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection property. Stellt eine Schätzung der Anzahl von Zeichen einschließlich Leerzeichen im Dokument dar"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/characterswithspaces/
---
## BuiltInDocumentPropertyCollection.CharactersWithSpaces property

Stellt eine Schätzung der Anzahl von Zeichen (einschließlich Leerzeichen) im Dokument dar.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CharactersWithSpaces { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersWithSpacesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf integrierte Dokumenteigenschaften
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Zeige den aktuellen CharactersWithSpaces-Wert an
            Console.WriteLine("Current CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Setze einen neuen Wert für CharactersWithSpaces
            properties.CharactersWithSpaces = 1500;
            Console.WriteLine("Updated CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Einige Inhalte hinzufügen, um die Wirkung der Eigenschaft zu demonstrieren
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            worksheet.Cells["A2"].PutValue("The CharactersWithSpaces property represents estimated character count including spaces.");
            
            // Speichere die Arbeitsmappe
            workbook.Save("PropertyCharactersWithSpacesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


