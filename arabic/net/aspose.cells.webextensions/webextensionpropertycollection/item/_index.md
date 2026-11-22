---
title: "WebExtensionPropertyCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionPropertyCollection. تحصل على خاصية web extension حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionpropertycollection/item/
---
## WebExtensionPropertyCollection indexer (1 of 2)

تحصل على خاصية web extension حسب الفهرس.

```csharp
public WebExtensionProperty this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

خاصية web extension.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة خصائص web extension
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // أضف بعض الخصائص
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // الوصول إلى الخصائص باستخدام فهرس العنصر
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // عدّل قيم الخصائص عبر المجموعة
            properties[index1].Value = "UpdatedValue1";
            properties[index2].Value = "UpdatedValue2";

            // اعرض التغييرات
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // احفظ المصنف (مع أن خصائص ملحق الويب لن تكون مرئية في الملف المحفوظ دون إعداد صحيح)
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)

---

## WebExtensionPropertyCollection indexer (2 of 2)

يحصل على خاصية ملحق الويب.

```csharp
public WebExtensionProperty this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم الخاصية. |

### قيمة الإرجاع

خاصية web extension.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة خصائص web extension
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // إضافة خصائص إلى المجموعة
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");

            // الوصول إلى الخصائص باستخدام الفهرس Item
            WebExtensionProperty property1 = properties["Property1"];
            Console.WriteLine("Property1 value: " + property1.Value);

            WebExtensionProperty property2 = properties["Property2"];
            Console.WriteLine("Property2 value: " + property2.Value);

            // عدّل قيم الخصائص (ملاحظة: Item للقراءة فقط، لذا نحتاج إلى استخدام Add/Remove)
            properties.RemoveAt("Property1");
            properties.Add("Property1", "NewValue1");

            // اعرض القيمة المحدثة
            property1 = properties["Property1"];
            Console.WriteLine("Updated Property1 value: " + property1.Value);

            // احفظ المصنف
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


