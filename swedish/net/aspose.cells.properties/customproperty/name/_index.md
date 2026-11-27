---
title: "CustomProperty.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomProperty property. Returnerar eller anger namnet på objektet"
type: docs
url: /sv/net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Returnerar eller anger namnet på objektet.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en anpassad egenskap med ett namn och ett värde
                worksheet.CustomProperties.Add("SampleName", "SampleValue");

                // Hämta den anpassade egenskapen
                CustomProperty customProperty = worksheet.CustomProperties["SampleName"];

                // Visa det aktuella värdet för Name-egenskapen (läsläsning)
                Console.WriteLine("Custom Property Name: " + customProperty.Name);

                // Ange ett nytt värde för Name-egenskapen
                customProperty.Name = "UpdatedName";
                Console.WriteLine("Updated Custom Property Name: " + customProperty.Name);

                // Spara arbetsboken
                workbook.Save("NameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


