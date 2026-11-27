---
title: "ContentTypeProperty.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ContentTypeProperty egenskap. Hämtar och anger typen för egenskapen"
type: docs
url: /sv/net/aspose.cells.properties/contenttypeproperty/type/
---
## ContentTypeProperty.Type property

Hämtar och anger typen för egenskapen.

```csharp
public string Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Lägg till innehållstyp-egenskaper med olika typer
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            workbook.ContentTypeProperties.Add("Version", "1.0", "number");
            workbook.ContentTypeProperties.Add("Enabled", "true", "boolean");

            // Få åtkomst till och visa egenskapstyper
            foreach (ContentTypeProperty property in workbook.ContentTypeProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

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


