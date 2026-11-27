---
title: "ContentTypePropertyCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ContentTypePropertyCollection egenskap. Hämtar innehållstyp-egenskapen med ett specifikt index"
type: docs
url: /sv/net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

Hämtar innehållstyp-egenskapen med ett specifikt index.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Innehållstyp-egenskapen

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Lägg till innehållstyp-egenskaper och demonstrera användning av Item-egenskapen
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Åtkomst till egenskaper med Item-indexerare
            Console.WriteLine($"Property1 IsNillable: {workbook.ContentTypeProperties[0].IsNillable}");
            Console.WriteLine($"Property2 IsNillable: {workbook.ContentTypeProperties[1].IsNillable}");
            
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Se även

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

Hämtar innehållstyp-egenskapen med egenskapsnamnet.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Egenskapsnamnet. |

### Returvärde

Innehållstyp-egenskapen

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Lägg till innehållstyp-egenskap
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Få åtkomst till egenskapen med Item-indexerare
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Ändra egenskapsvärden
            property.Value = "UpdatedValue";
            property.IsNillable = false;
            
            // Spara arbetsbok
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


