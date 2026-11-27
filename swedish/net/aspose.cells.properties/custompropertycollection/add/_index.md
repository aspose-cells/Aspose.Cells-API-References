---
title: "CustomPropertyCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomPropertyCollection-metoden. Lägger till information om anpassad egenskap"
type: docs
url: /sv/net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

Lägger till information om anpassad egenskap.

```csharp
public int Add(string name, string value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på den anpassade egenskapen. |
| värde | String | Värdet på den anpassade egenskapen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomPropertyCollection customProperties = worksheet.CustomProperties;
            
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");

            foreach (CustomProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### Se även

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


