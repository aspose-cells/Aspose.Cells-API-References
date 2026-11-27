---
title: "Workbook.ContentTypeProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar listan med ContentTypeProperty-objekt i workbook"
type: docs
url: /sv/net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

Hämtar listan med [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) objekt i workbook.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyContentTypePropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Lägg till enkel strängegenskap
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            // Lägg till datetime-egenskap med typspecifikation
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Spara arbetsboken
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Se även

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


