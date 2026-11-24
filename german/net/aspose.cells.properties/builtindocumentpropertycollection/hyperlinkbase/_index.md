---
title: "BuiltInDocumentPropertyCollection.HyperlinkBase"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection property. Liest oder setzt die hyperlinkbase-Eigenschaft"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/hyperlinkbase/
---
## BuiltInDocumentPropertyCollection.HyperlinkBase property

Liest oder setzt die hyperlinkbase‑Eigenschaft.

```csharp
public string HyperlinkBase { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyHyperlinkBaseDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Setze die HyperlinkBase-Eigenschaft
            workbook.BuiltInDocumentProperties.HyperlinkBase = "http://www.example.com";

            // Setze eine weitere Eigenschaft zur Demonstration
            workbook.BuiltInDocumentProperties.Title = "Sample Workbook";

            // Speichere die Arbeitsmappe
            workbook.Save("HyperlinkBaseDemo.xlsx", SaveFormat.Xlsx);

            // Laden der gespeicherten Arbeitsmappe, um Eigenschaften zu überprüfen
            Workbook loadedWorkbook = new Workbook("HyperlinkBaseDemo.xlsx");
            
            // Gib die Eigenschaften in der Konsole aus
            Console.WriteLine("HyperlinkBase: " + loadedWorkbook.BuiltInDocumentProperties.HyperlinkBase);
            Console.WriteLine("Title: " + loadedWorkbook.BuiltInDocumentProperties.Title);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


