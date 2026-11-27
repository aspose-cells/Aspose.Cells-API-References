---
title: "CustomProperty.StringValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomProperty-egenskapen. Returnerar eller anger värdet på den anpassade egenskapen"
type: docs
url: /sv/net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

Returnerar eller anger värdet för den anpassade egenskapen.

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen CustomProperty.Value. Denna egenskap kommer att tas bort 12 månader senare sedan juni 2010. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en anpassad egenskap med ett strängvärde
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // Hämta den anpassade egenskapen
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // Visa StringValue-egenskapen (läsläsning)
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // Ange ett nytt värde för StringValue-egenskapen
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // Spara arbetsboken
                workbook.Save("StringValueDemo.xlsx");
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


