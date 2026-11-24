---
title: "ContentTypePropertyCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ContentTypePropertyCollection-Methode. Fügt Informationen zu Content-Type-Eigenschaften hinzu"
type: docs
url: /de/net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

Fügt Informationen zur Content‑Typ‑Eigenschaft hinzu.

```csharp
public int Add(string name, string value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Content-Type-Eigenschaft. |
| Wert | String | Der Wert der Content-Type-Eigenschaft. |

### Beispiele

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

### Siehe auch

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

Fügt Informationen zur Content‑Typ‑Eigenschaft hinzu.

```csharp
public int Add(string name, string value, string type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Content-Type-Eigenschaft. |
| Wert | String | Der Wert der Content-Type-Eigenschaft. |
| Typ | String | Der Typ der Content-Type-Eigenschaft. |

### Beispiele

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

### Siehe auch

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


