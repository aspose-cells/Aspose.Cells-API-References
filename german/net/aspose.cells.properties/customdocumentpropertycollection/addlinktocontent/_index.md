---
title: "CustomDocumentPropertyCollection.AddLinkToContent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomDocumentPropertyCollection-Methode. Erstellt eine neue benutzerdefinierte Dokumenteigenschaft, die mit Inhalt verknüpft ist"
type: docs
url: /de/net/aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/
---
## CustomDocumentPropertyCollection.AddLinkToContent method

Erstellt eine neue benutzerdefinierte Dokumenteigenschaft, die mit Inhalt verknüpft ist.

```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Eigenschaft. |
| source | String | Die Quelle der Eigenschaft. Sie sollte der Name des benannten Bereichs sein. |

### Rückgabewert

Das neu erstellte Eigenschaftsobjekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddLinkToContentWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie einen Wert in Zelle A1, der verknüpft wird
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Fügen Sie eine reguläre Eigenschaft zum Vergleich hinzu
            customProperties.Add("RegularProperty", "Static Value");
            
            // Verknüpfte Eigenschaft hinzufügen
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
            
            // Verknüpften Wert aktualisieren
            customProperties.UpdateLinkedRange();

            // Zeigen Sie die Eigenschaften an
            Console.WriteLine($"Regular Property: {customProperties["RegularProperty"].Value}");
            Console.WriteLine($"Linked Property: {customProperties["LinkedProperty"].Value}");

            workbook.Save("LinkedPropertyExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


