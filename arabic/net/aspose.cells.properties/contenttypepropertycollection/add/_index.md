---
title: "ContentTypePropertyCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ContentTypePropertyCollection. تُضيف معلومات خاصية نوع المحتوى"
type: docs
url: /ar/net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

يضيف معلومات خاصية نوع المحتوى.

```csharp
public int Add(string name, string value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم خاصية نوع المحتوى. |
| القيمة | String | قيمة خاصية نوع المحتوى. |

### أمثلة

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

### انظر أيضًا

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

يضيف معلومات خاصية نوع المحتوى.

```csharp
public int Add(string name, string value, string type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم خاصية نوع المحتوى. |
| القيمة | String | قيمة خاصية نوع المحتوى. |
| type | String | نوع خاصية نوع المحتوى. |

### أمثلة

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

### انظر أيضًا

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


