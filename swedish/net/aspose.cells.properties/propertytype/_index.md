---
title: "Enum PropertyType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Properties.PropertyType enum. Anger datatyp för en dokumentegenskap"
type: docs
url: /sv/net/aspose.cells.properties/propertytype/
---
## PropertyType enumeration

Anger datatyp för en dokumentegenskap.

```csharp
public enum PropertyType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Boolean | `0` | Egenskapen är ett booleskt värde. |
| DateTime | `1` | Egenskapen är ett datum-tidsvärde. |
| Double | `2` | Egenskapen är ett flyttal. |
| Number | `3` | Egenskapen är ett heltal. |
| String | `4` | Egenskapen är ett strängvärde. |
| Blob | `5` | Egenskapen är en byte-array |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class PropertyTypeDemo
    {
        public static void PropertyTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till de inbyggda dokumentegenskaperna
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ställ in några inbyggda egenskaper
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // Åtkomst till de anpassade dokumentegenskaperna
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Lägg till anpassade egenskaper av olika typer
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // Hämta och visa anpassade egenskaper
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Spara arbetsboken
            workbook.Save("PropertyTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


