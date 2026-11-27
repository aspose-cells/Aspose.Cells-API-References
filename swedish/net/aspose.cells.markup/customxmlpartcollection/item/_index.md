---
title: "CustomXmlPartCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomXmlPartCollection egenskap. Hämtar ett objekt på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.markup/customxmlpartcollection/item/
---
## CustomXmlPartCollection indexer

Hämtar ett objekt på det angivna indexet.

```csharp
public CustomXmlPart this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till CustomXmlPartCollection direkt från Workbook
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Exempel på XML-data
            string xmlData = "<root><item>Test Data</item></root>";
            byte[] xmlBytes = System.Text.Encoding.UTF8.GetBytes(xmlData);
            
            // Lägg till en anpassad XML-del
            int index = customXmlParts.Add(xmlBytes, null);
            
            // Åtkomst till objektet med Item-egenskapen
            CustomXmlPart part = customXmlParts[index];
            
            // Visa ID för den anpassade XML-delen
            Console.WriteLine("Custom XML Part ID: " + part.ID);
            
            // Hämta XML-data tillbaka från delen
            string retrievedXml = System.Text.Encoding.UTF8.GetString(part.Data);
            Console.WriteLine("XML Content: " + retrievedXml);
            
            // Spara arbetsboken
            workbook.Save("CustomXmlPartDemo.xlsx");
        }
    }
}
```

### Se även

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


