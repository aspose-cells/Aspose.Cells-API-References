---
title: "Klass CustomProperty"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Properties.CustomProperty‑klass. Representerar en anpassad egenskap som lagrar namn‑ och värdepar av godtycklig användardefinierad data för arbetsbladet"
type: docs
url: /sv/net/aspose.cells.properties/customproperty/
---
## CustomProperty class

Representerar en anpassad egenskap som lagrar namn‑ och värdepar av godtycklig användardefinierad data för kalkylblad.

```csharp
public class CustomProperty
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BinaryValue](../../aspose.cells.properties/customproperty/binaryvalue/) { get; set; } | Hämtar och anger det binära värdet för den anpassade egenskapen. |
| [Name](../../aspose.cells.properties/customproperty/name/) { get; set; } | Returnerar eller anger namnet på objektet. |
| [StringValue](../../aspose.cells.properties/customproperty/stringvalue/) { get; set; } | (**Obsolete.**) Returnerar eller anger värdet för den anpassade egenskapen. |
| [Value](../../aspose.cells.properties/customproperty/value/) { get; set; } | Returnerar eller anger värdet för den anpassade egenskapen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyDemo
    {
        public static void CustomPropertyExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Åtkomst till samlingen CustomProperties
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Lägg till anpassade egenskaper
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // Åtkomst och visning av anpassade egenskaper
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Spara arbetsboken
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


