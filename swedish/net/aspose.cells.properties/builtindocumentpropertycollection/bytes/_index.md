---
title: "BuiltInDocumentPropertyCollection.Bytes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection property. Representerar en uppskattning av antalet byte i dokumentet"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/bytes/
---
## BuiltInDocumentPropertyCollection.Bytes property

Representerar en uppskattning av antalet byte i dokumentet.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Bytes { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyBytesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Visa aktuellt Bytes‑värde (uppskattning av dokumentstorlek)
            Console.WriteLine("Current Bytes value: " + properties.Bytes);

            // Lägg till lite innehåll för att påverka storleken
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data to increase document size");
            for (int i = 2; i <= 100; i++)
            {
                worksheet.Cells["A" + i].PutValue("Line " + i);
            }

            // Uppdatera Bytes‑egenskapen manuellt (även om den normalt beräknas automatiskt)
            properties.Bytes = 5000;
            Console.WriteLine("Updated Bytes value: " + properties.Bytes);

            // Spara arbetsboken för att se egenskapen i den sparade filen
            workbook.Save("PropertyBytesDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


