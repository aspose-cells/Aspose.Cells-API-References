---
title: "ContentTypeProperty.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ContentTypeProperty-egenskap. Returnerar eller anger namnet på objektet"
type: docs
url: /sv/net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

Returnerar eller anger namnet på objektet.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en innehållstypsegenskap med namnet "ss"
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            
            // Spara i XLS-format
            workbook.Save("example.xls");
            
            // Läs in arbetsboken igen och verifiera Name-egenskapen
            workbook = new Workbook("example.xls");
            Console.WriteLine("Name property in XLS: " + workbook.ContentTypeProperties[0].Name);
            
            // Spara i XLSX-format
            workbook.Save("example.xlsx");
            
            // Läs in igen och verifiera igen
            workbook = new Workbook("example.xlsx");
            Console.WriteLine("Name property in XLSX: " + workbook.ContentTypeProperties[0].Name);
        }
    }
}
```

### Se även

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


