---
title: "SmartTagPropertyCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SmartTagPropertyCollection. تحصل على كائن SmartTagProperty"
type: docs
url: /ar/net/aspose.cells.markup/smarttagpropertycollection/item/
---
## SmartTagPropertyCollection indexer (1 of 2)

تحصل على كائن [`SmartTagProperty`](../../smarttagproperty/)

```csharp
public SmartTagProperty this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس |

### قيمة الإرجاع

يرجع كائنًا من نوع [`SmartTagProperty`](../../smarttagproperty/).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة خصائص للعلامة الذكية
            SmartTagPropertyCollection properties = new SmartTagPropertyCollection();

            // إضافة خصائص إلى المجموعة
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // الوصول إلى الخصائص باستخدام فهرس العنصر
            SmartTagProperty property1 = properties[index1];
            SmartTagProperty property2 = properties[index2];

            // عرض قيم الخصائص الحالية
            Console.WriteLine("Property1 Name: " + property1.Name);
            Console.WriteLine("Property1 Value: " + property1.Value);
            Console.WriteLine("Property2 Name: " + property2.Name);
            Console.WriteLine("Property2 Value: " + property2.Value);

            // ملاحظة: خاصية Item للقراءة فقط، لذا لا يمكننا تعيينها مباشرة
            // بدلاً من ذلك، يمكننا تعديل خصائص كائنات SmartTagProperty المعادة
            property1.Value = "UpdatedValue1";
            property2.Value = "UpdatedValue2";

            // عرض القيم المحدثة
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property1 Value: " + properties[index1].Value);
            Console.WriteLine("Property2 Value: " + properties[index2].Value);

            // حفظ المصنف (على الرغم من أن العلامات الذكية لا تُحفظ بشكل مرئي في حفظ بسيط)
            workbook.Save("SmartTagPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagPropertyCollection indexer (2 of 2)

يحصل على كائن [`SmartTagProperty`](../../smarttagproperty/) بحسب اسم الخاصية.

```csharp
public SmartTagProperty this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم الخاصية. |

### قيمة الإرجاع

يرجع كائنًا من نوع [`SmartTagProperty`](../../smarttagproperty/).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء إعداد للعلامة الذكية وإضافة علامة ذكية
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
                int smartTagIndex = smartTagSetting.Add(0, 0);
                SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
                smartTags.Add("http://example.com", "example");

                // احصل على العلامة الذكية وخصائصها
                SmartTag smartTag = smartTags[0];
                SmartTagPropertyCollection properties = smartTag.Properties;

                // إضافة بعض الخصائص لتوضيح خاصية Item
                properties.Add("Author", "John Doe");
                properties.Add("Version", "1.0");

                // الوصول إلى الخصائص باستخدام الفهرس Item (حسب الفهرس)
                SmartTagProperty firstProperty = properties[0];
                SmartTagProperty secondProperty = properties[1];

                // عرض قيم الخصائص
                Console.WriteLine("First Property Name: " + firstProperty.Name);
                Console.WriteLine("First Property Value: " + firstProperty.Value);
                Console.WriteLine("Second Property Name: " + secondProperty.Name);
                Console.WriteLine("Second Property Value: " + secondProperty.Value);

                // احفظ المصنف
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


