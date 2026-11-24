---
title: "BuiltInDocumentPropertyCollection.LastPrinted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Gibt das Datum zurück, an dem das Dokument zuletzt in der lokalen Zeitzone gedruckt wurde, oder legt es fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinted/
---
## BuiltInDocumentPropertyCollection.LastPrinted property

Liest oder setzt das Datum, an dem das Dokument zuletzt in der lokalen Zeitzone gedruckt wurde.

```csharp
public DateTime LastPrinted { get; set; }
```

### Hinweise

Wenn das Dokument nie gedruckt wurde, gibt diese Eigenschaft DateTime.MinValue zurück.

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Integrierte Dokumenteigenschaften festlegen
            workbook.BuiltInDocumentProperties.CreatedTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now.AddDays(-1); // Set to yesterday
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Die Eigenschaft LastPrinted anzeigen
            Console.WriteLine("Last printed: " + workbook.BuiltInDocumentProperties.LastPrinted);

            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


