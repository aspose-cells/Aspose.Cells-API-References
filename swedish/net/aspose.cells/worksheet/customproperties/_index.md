---
title: "Worksheet.CustomProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Kalkylbladsattribut. Hämtar ett objekt som representerar identifieringsinformationen som är associerad med ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Hämtar ett objekt som representerar identifieringsinformationen som är associerad med ett kalkylblad.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Anmärkningar

Worksheet.CustomProperties erbjuder en föredragen mekanism för att lagra godtyckliga data. Det stöder äldre tredjepartsdokumentkomponenter, samt situationer som har ett strikt behov av binära delar.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCustomPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till anpassade egenskaper i kalkylbladet
            worksheet.CustomProperties.Add("Property1", "Value1");
            worksheet.CustomProperties.Add("Property2", "12345");
            worksheet.CustomProperties.Add("Property3", DateTime.Now.ToString());
            
            // Visa antal anpassade egenskaper
            Console.WriteLine("Custom Properties Count: " + worksheet.CustomProperties.Count);
            
            // Kom åt och visa egenskapsvärden
            foreach (var prop in worksheet.CustomProperties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
            }
            
            // Spara arbetsboken
            workbook.Save("WorksheetCustomPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


