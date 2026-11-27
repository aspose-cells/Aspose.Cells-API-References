---
title: "ContentTypeProperty.IsNillable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ContentTypeProperty egenskap. Anger om värdet kan vara tomt"
type: docs
url: /sv/net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Indikerar om värdet kan vara tomt.

```csharp
public bool IsNillable { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyIsNillableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Lägg till en innehållstypsegenskap
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Få åtkomst till egenskapen och sätt IsNillable
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.IsNillable = true;
            
            // Verifiera och skriv ut IsNillable-värdet
            Console.WriteLine($"Property 'Admin' IsNillable: {property.IsNillable}");
            
            workbook.Save("ContentTypePropertyIsNillableDemo.xlsx");
        }
    }
}
```

### Se även

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


