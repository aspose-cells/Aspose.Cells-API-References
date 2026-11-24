---
title: "DocumentProperty.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Eigenschaft. Gibt den Wert der Eigenschaft zurück oder setzt ihn"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

Ermittelt oder setzt den Wert der Eigenschaft.

```csharp
public object Value { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf integrierte Dokumenteigenschaften
            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.example.com";

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "Sample Document Title";

            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertiesDemo.xlsx");

            // Zeige die gesetzten Werte an
            Console.WriteLine("HyperlinkBase: " + hyperlinkBase.Value);
            Console.WriteLine("Title: " + title.Value);
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


