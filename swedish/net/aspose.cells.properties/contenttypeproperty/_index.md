---
title: "Klass ContentTypeProperty"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Properties.ContentTypeProperty-klass. Representerar identifieringsinformation"
type: docs
url: /sv/net/aspose.cells.properties/contenttypeproperty/
---
## ContentTypeProperty class

Representerar identifieringsinformation.

```csharp
public class ContentTypeProperty
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | Indikerar om värdet kan vara tomt. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | Returnerar eller anger namnet på objektet. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | Hämtar och anger typen för egenskapen. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | Returnerar eller anger värdet för innehållstypsegenskapen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyDemo
    {
        public static void ContentTypePropertyExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Lägg till en ny innehållstypsegenskap
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Åtkomst till den nyligen tillagda egenskapen
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Ställa in egenskaper
            property.Name = "Admin";
            property.Value = "Aspose";
            property.Type = "text";
            property.IsNillable = true;

            // Spara Excel-filen
            workbook.Save("ContentTypePropertyExample.xlsx");
            workbook.Save("ContentTypePropertyExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


