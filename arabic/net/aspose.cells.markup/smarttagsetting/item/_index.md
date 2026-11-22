---
title: "SmartTagSetting.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SmartTagSetting. تحصل على كائن SmartTagCollection حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.markup/smarttagsetting/item/
---
## SmartTagSetting indexer (1 of 3)

يحصل على كائن [`SmartTagCollection`](../../smarttagcollection/) حسب الفهرس.

```csharp
public SmartTagCollection this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| index | فهرس كائن [`SmartTagCollection`](../../smarttagcollection/) في القائمة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            
            // عرض استخدام خاصية Item
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
            smartTags.Add("http://docs.aspose.com", "docs");
            
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Version", "1.0");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (2 of 3)

يحصل على كائن [`SmartTagCollection`](../../smarttagcollection/) للخلية.

```csharp
public SmartTagCollection this[int row, int column] { get; }
```

| معامل | الوصف |
| --- | --- |
| صف | فهرس الصف للخلية. |
| عمود | فهرس العمود للخلية |

### قيمة الإرجاع

يعيد كائن [`SmartTagCollection`](../../smarttagcollection/) للخلية. يعيد null إذا لم توجد أي علامات ذكية في الخلية.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            // عرض استخدام خاصية Item
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart tags in cell A1: " + smartTagCollection.Count);
            Console.WriteLine("Namespace URI: " + smartTagCollection[0].Uri);
            Console.WriteLine("Tag name: " + smartTagCollection[0].Name);

            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (3 of 3)

يحصل على كائن [`SmartTagCollection`](../../smarttagcollection/) للخلية.

```csharp
public SmartTagCollection this[string cellName] { get; }
```

| معامل | الوصف |
| --- | --- |
| cellName | اسم الخلية. |

### قيمة الإرجاع

يعيد كائن [`SmartTagCollection`](../../smarttagcollection/) للخلية. يعيد null إذا لم توجد أي علامات ذكية في الخلية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingPropertyItemDemo2
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // احصل على ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // الوصول إلى SmartTagSetting لورقة العمل
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;

                // أضف علامة ذكية إلى الخلية A1 (الصف 0، العمود 0)
                int smartTagIndex = smartTagSetting.Add(0, 0);

                // إظهار استخدام خاصية Item (المؤشر)
                SmartTagCollection smartTagCollection = smartTagSetting[smartTagIndex];

                // إضافة علامة ذكية إلى المجموعة
                smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

                // عرض معلومات حول العلامة الذكية
                Console.WriteLine("Number of smart tags in collection: " + smartTagCollection.Count);
                if (smartTagCollection.Count > 0)
                {
                    Console.WriteLine("First smart tag URI: " + smartTagCollection[0].Uri);
                    Console.WriteLine("First smart tag name: " + smartTagCollection[0].Name);
                }

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

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


