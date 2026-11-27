---
title: "CustomProperty.BinaryValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomProperty-egenskap. Hämtar och sätter det binära värdet för den anpassade egenskapen"
type: docs
url: /sv/net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

Hämtar och anger det binära värdet för den anpassade egenskapen.

```csharp
public byte[] BinaryValue { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en anpassad egenskap med ett exempelvärde
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // Hämta den anpassade egenskapen
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // Visa Name och Value för den anpassade egenskapen
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // OBS: Reflektionen för CustomProperty inkluderar inte en BinaryValue-egenskap.
                // Det tillgängliga strängbaserade värdet nås via egenskapen 'Value'.

                // Spara arbetsboken (valfritt)
                workbook.Save("BinaryValueDemo.xlsx");
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


