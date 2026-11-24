---
title: "CustomDocumentPropertyCollection.UpdateLinkedRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomDocumentPropertyCollection-Methode. Aktualisiert alle Bereiche, die mit benutzerdefinierten Eigenschaften verknüpft sind, und verwendet den Wert der benutzerdefinierten Dokumenteigenschaft, um den Zellenwert des verknüpften Bereichs zu aktualisieren."
type: docs
url: /de/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/
---
## CustomDocumentPropertyCollection.UpdateLinkedRange method

Aktualisiert alle Bereiche, die mit benutzerdefinierten Eigenschaften verknüpft sind (Verwenden Sie den Wert der benutzerdefinierten Dokumenteigenschaft, um den Zellenwert des verknüpften Bereichs zu aktualisieren).

```csharp
public void UpdateLinkedRange()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie einen Wert in Zelle A1, der verknüpft wird
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Verknüpfte Eigenschaft hinzufügen
            customProperties.AddLinkToContent("LinkedRange", "Sheet1!A1");
            
            // Alle verknüpften Eigenschaften aktualisieren
            customProperties.UpdateLinkedRange();
            
            // Verknüpften Eigenschaftswert abrufen und anzeigen
            DocumentProperty linkedProp = customProperties["LinkedRange"];
            Console.WriteLine($"Linked Property Value: {linkedProp.Value}");

            // Speichere die Arbeitsmappe
            workbook.Save("LinkedRangeExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


