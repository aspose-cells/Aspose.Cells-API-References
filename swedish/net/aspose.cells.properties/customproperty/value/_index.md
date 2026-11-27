---
title: "CustomProperty.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomProperty-egenskapen. Returnerar eller anger värdet på den anpassade egenskapen"
type: docs
url: /sv/net/aspose.cells.properties/customproperty/value/
---
## CustomProperty.Value property

Returnerar eller anger värdet för den anpassade egenskapen.

```csharp
public string Value { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en anpassad egenskap med ett långt strängvärde
            worksheet.CustomProperties.Add("VeryLongString", "This is a very long string value for testing custom properties");
            
            // Hämta och visa värdet på den anpassade egenskapen
            string propertyValue = worksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Custom Property Value: " + propertyValue);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in arbetsboken igen för att verifiera att egenskapen kvarstår
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Verifiera att värdet är detsamma efter inläsning
            string loadedValue = loadedWorksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Reloaded Custom Property Value: " + loadedValue);
        }
    }
}
```

### Se även

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


