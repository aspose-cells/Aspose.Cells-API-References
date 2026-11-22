---
title: "DocumentPropertyCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocumentPropertyCollection. تُرجع كائن DocumentProperty باسم الخاصية."
type: docs
url: /ar/net/aspose.cells.properties/documentpropertycollection/item/
---
## DocumentPropertyCollection indexer (1 of 2)

تُرجع كائن [`DocumentProperty`](../../documentproperty/) باسم الخاصية.

```csharp
public virtual DocumentProperty this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم الخاصية غير حساس لحالة الأحرف المراد استرجاعه. |

### ملاحظات

يرجع null إذا لم يتم العثور على خاصية بالاسم المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            string key = "TemplateGUID";
            object value = "TestValue123";

            if (wb.Worksheets.CustomDocumentProperties.Contains(key))
            {
                wb.Worksheets.CustomDocumentProperties[key].Value = value;
            }
            else
            {
                wb.Worksheets.CustomDocumentProperties.Add(key, value.ToString());
            }

            // تحقق من أن القيمة تم تعيينها باستخدام خاصية Item
            Console.WriteLine("Property Value: " + wb.Worksheets.CustomDocumentProperties[key].Value);
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## DocumentPropertyCollection indexer (2 of 2)

يرجع كائن [`DocumentProperty`](../../documentproperty/) حسب الفهرس.

```csharp
public DocumentProperty this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| index | الفهرس الصفري لـ [`DocumentProperty`](../../documentproperty/) المراد استرجاعه. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // عيّن الخصائص المدمجة (ليس إضافة)
            properties.Author = "John Doe";
            properties.Company = "Aspose";
            properties["Version"].Value = "1.0";

            // الوصول إلى الخصائص باستخدام فهرس العنصر
            Console.WriteLine("Property 0: " + properties[0].Name + " = " + properties[0].Value);
            Console.WriteLine("Property 1: " + properties[1].Name + " = " + properties[1].Value);
            Console.WriteLine("Property 2: " + properties[2].Name + " = " + properties[2].Value);

            // الوصول إلى الخاصية حسب الاسم
            DocumentProperty authorProp = properties["Author"];
            Console.WriteLine("Author property: " + authorProp.Value);

            // تعديل خاصية
            properties["Version"].Value = "2.0";
            Console.WriteLine("Updated Version: " + properties["Version"].Value);
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


