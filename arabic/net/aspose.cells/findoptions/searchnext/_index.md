---
title: "FindOptions.SearchNext"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. ترتيب البحث. True للبحث التالي. False للبحث السابق"
type: docs
url: /ar/net/aspose.cells/findoptions/searchnext/
---
## FindOptions.SearchNext property

ترتيب البحث. True: البحث التالي. False: البحث السابق.

```csharp
[Obsolete("Use FindOptions.SearchBackward property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SearchNext { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية FindOptions.SearchBackward. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2018. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertySearchNextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ بعض بيانات العينة
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("apple pie");

            // إنشاء خيارات البحث
            FindOptions findOptions = new FindOptions();
            findOptions.CaseSensitive = false;
            findOptions.LookAtType = LookAtType.Contains;

            // عرض خاصية SearchNext (مهجور، ولكن معروض للتوضيح)
            Console.WriteLine("Initial SearchNext value: " + findOptions.SearchNext);
            
            // البحث إلى الأمام (السلوك الافتراضي)
            findOptions.SearchNext = true;
            Cell firstForward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First forward search result: " + (firstForward != null ? firstForward.Name + " - " + firstForward.StringValue : "Not found"));

            // بحث إلى الخلف
            findOptions.SearchNext = false;
            Cell firstBackward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First backward search result: " + (firstBackward != null ? firstBackward.Name + " - " + firstBackward.StringValue : "Not found"));

            // احفظ المصنف
            workbook.Save("PropertySearchNextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


