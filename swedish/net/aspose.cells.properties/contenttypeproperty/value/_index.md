---
title: "ContentTypeProperty.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ContentTypeProperty-egenskap. Returnerar eller anger värdet för innehållstypens egenskap"
type: docs
url: /sv/net/aspose.cells.properties/contenttypeproperty/value/
---
## ContentTypeProperty.Value property

Returnerar eller anger värdet för innehållstypsegenskapen.

```csharp
public string Value { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Lägg till en innehållstypsegenskap
            workbook.ContentTypeProperties.Add("Admin", "InitialValue", "text");
            
            // Kom åt och ändra egenskapens värde
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.Value = "Aspose"; // Demonstrating Value property usage
            
            // Spara arbetsboken
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


