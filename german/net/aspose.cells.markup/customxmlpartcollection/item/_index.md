---
title: "CustomXmlPartCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomXmlPartCollection-Eigenschaft. Gibt ein Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.markup/customxmlpartcollection/item/
---
## CustomXmlPartCollection indexer

Liefert ein Element am angegebenen Index.

```csharp
public CustomXmlPart this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class CustomXmlPartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie direkt auf die CustomXmlPartCollection aus der Arbeitsmappe zu
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Beispieldaten für XML
            string xmlData = "<root><item>Test Data</item></root>";
            byte[] xmlBytes = System.Text.Encoding.UTF8.GetBytes(xmlData);
            
            // Fügen Sie ein benutzerdefiniertes XML-Teil hinzu
            int index = customXmlParts.Add(xmlBytes, null);
            
            // Greifen Sie über die Item-Eigenschaft auf das Element zu
            CustomXmlPart part = customXmlParts[index];
            
            // Zeigen Sie die ID des benutzerdefinierten XML-Teils an
            Console.WriteLine("Custom XML Part ID: " + part.ID);
            
            // Holen Sie die XML-Daten aus dem Teil zurück
            string retrievedXml = System.Text.Encoding.UTF8.GetString(part.Data);
            Console.WriteLine("XML Content: " + retrievedXml);
            
            // Speichere die Arbeitsmappe
            workbook.Save("CustomXmlPartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


