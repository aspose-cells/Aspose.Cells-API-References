---
title: "ContentTypePropertyCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ContentTypePropertyCollection-metod. Lägger till information om innehållstyp-egenskap"
type: docs
url: /sv/net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

Lägger till information om innehållstypsegenskap.

```csharp
public int Add(string name, string value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på innehållstyp-egenskapen. |
| värde | String | Värdet på innehållstyp-egenskapen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            ContentTypePropertyCollection ctps = wb.ContentTypeProperties;
            ctps.Add("CustomProperty1", "SampleValue1");
            ctps.Add("CustomProperty2", "SampleValue2");
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

Lägger till information om innehållstypsegenskap.

```csharp
public int Add(string name, string value, string type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på innehållstyp-egenskapen. |
| värde | String | Värdet på innehållstyp-egenskapen. |
| typ | String | Typen av innehållstyp-egenskapen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.ContentTypeProperties.Add("propertyName", "propertyValue", "string");
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


