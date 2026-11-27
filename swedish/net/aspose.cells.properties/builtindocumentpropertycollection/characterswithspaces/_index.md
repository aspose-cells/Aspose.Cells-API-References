---
title: "BuiltInDocumentPropertyCollection.CharactersWithSpaces"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Representerar en uppskattning av antalet tecken inklusive mellanslag i dokumentet"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/characterswithspaces/
---
## BuiltInDocumentPropertyCollection.CharactersWithSpaces property

Representerar en uppskattning av antalet tecken (inklusive mellanslag) i dokumentet.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CharactersWithSpaces { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Visa aktuellt värde för CharactersWithSpaces
            Console.WriteLine("Current CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Ange ett nytt värde för CharactersWithSpaces
            properties.CharactersWithSpaces = 1500;
            Console.WriteLine("Updated CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Lägg till lite innehåll för att demonstrera egenskapseffekten
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            worksheet.Cells["A2"].PutValue("The CharactersWithSpaces property represents estimated character count including spaces.");
            
            // Spara arbetsboken
            workbook.Save("PropertyCharactersWithSpacesDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


