---
title: "ContentTypePropertyCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ContentTypePropertyCollection. يحصل على خاصية نوع المحتوى بواسطة الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

يحصل على خاصية نوع المحتوى بواسطة الفهرس المحدد.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

خاصية نوع المحتوى

### أمثلة

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
            
            // إضافة خصائص نوع المحتوى وتوضيح استخدام خاصية Item
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // الوصول إلى الخصائص باستخدام فهرس العنصر
            Console.WriteLine($"Property1 IsNillable: {workbook.ContentTypeProperties[0].IsNillable}");
            Console.WriteLine($"Property2 IsNillable: {workbook.ContentTypeProperties[1].IsNillable}");
            
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

يحصل على خاصية نوع المحتوى بواسطة اسم الخاصية.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم الخاصية. |

### قيمة الإرجاع

خاصية نوع المحتوى

### أمثلة

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
            
            // إضافة خاصية نوع المحتوى
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // الوصول إلى الخاصية باستخدام الفهرس Item
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // تعديل قيم الخاصية
            property.Value = "UpdatedValue";
            property.IsNillable = false;
            
            // احفظ دفتر العمل
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


