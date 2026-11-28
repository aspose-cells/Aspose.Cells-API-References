---
title: "ContentTypePropertyCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ContentTypePropertyCollection yöntemi. İçerik türü özelliği bilgisi ekler"
type: docs
url: /tr/net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

İçerik türü özelliği bilgisi ekler.

```csharp
public int Add(string name, string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | İçerik türü özelliğinin adı. |
| değer | String | İçerik türü özelliğinin değeri. |

### Örnekler

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

### Ayrıca Bakınız

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

İçerik türü özelliği bilgisi ekler.

```csharp
public int Add(string name, string value, string type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | İçerik türü özelliğinin adı. |
| değer | String | İçerik türü özelliğinin değeri. |
| type | String | İçerik türü özelliğinin tipi. |

### Örnekler

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

### Ayrıca Bakınız

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


