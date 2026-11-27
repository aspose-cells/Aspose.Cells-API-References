---
title: "BuiltInDocumentPropertyCollection.Paragraphs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Representerar en uppskattning av antalet stycken i dokumentet"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/paragraphs/
---
## BuiltInDocumentPropertyCollection.Paragraphs property

Representerar en uppskattning av antalet stycken i dokumentet.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Paragraphs { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Visa aktuellt Paragraphs value (föråldrad egenskap)
            Console.WriteLine("Current Paragraphs value: " + properties.Paragraphs);

            // Ange ett nytt värde för Paragraphs (föråldrad egenskap)
            properties.Paragraphs = 15;
            Console.WriteLine("Updated Paragraphs value: " + properties.Paragraphs);

            // Lägg till lite innehåll för att demonstrera egenskapseffekten
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is paragraph 1");
            worksheet.Cells["A2"].PutValue("This is paragraph 2");
            worksheet.Cells["A3"].PutValue("This is paragraph 3");

            // Spara arbetsboken
            workbook.Save("PropertyParagraphsDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


