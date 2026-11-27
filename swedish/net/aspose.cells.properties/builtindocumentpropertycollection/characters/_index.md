---
title: "BuiltInDocumentPropertyCollection.Characters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Representerar en uppskattning av antalet tecken i dokumentet"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/characters/
---
## BuiltInDocumentPropertyCollection.Characters property

Representerar en uppskattning av antalet tecken i dokumentet.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Characters { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Visa aktuellt Characters‑värde (föråldrad egenskap)
            Console.WriteLine("Current Characters value: " + properties.Characters);

            // Ange ett nytt värde för Characters (föråldrad egenskap)
            properties.Characters = 1500;
            Console.WriteLine("Updated Characters value: " + properties.Characters);

            // Lägg till lite innehåll för att demonstrera egenskapseffekten
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            
            // Spara arbetsboken
            workbook.Save("PropertyCharactersDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


