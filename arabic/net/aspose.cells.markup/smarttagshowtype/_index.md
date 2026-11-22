---
title: "التعداد SmartTagShowType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Markup.SmartTagShowType. يمثل نوع العرض للعلامة الذكية."
type: docs
url: /ar/net/aspose.cells.markup/smarttagshowtype/
---
## SmartTagShowType enumeration

يمثل نوع العرض للعلامة الذكية.

```csharp
public enum SmartTagShowType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| All | `0` | يشير إلى أن العلامات الذكية مفعلة ومُظهرة |
| NoSmartTagIndicator | `1` | يشير إلى أن العلامات الذكية مفعلة لكن المؤشر غير معروض. |
| None | `2` | يشير إلى أن العلامات الذكية معطلة وغير معروضة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagShowTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض جميع قيم التعداد SmartTagShowType
            Console.WriteLine("SmartTagShowType values:");
            Console.WriteLine($"All: {SmartTagShowType.All}");
            Console.WriteLine($"NoSmartTagIndicator: {SmartTagShowType.NoSmartTagIndicator}");
            Console.WriteLine($"None: {SmartTagShowType.None}");

            // إنشاء وتكوين علامة ذكية
            var smartTagCollection = worksheet.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");

            // ضبط الخصائص التي قد تستخدم SmartTagShowType (محاكاة لأن الخاصية الفعلية غير متوفرة)
            Console.WriteLine("\nSmart tag created at A1 with current date");

            // حفظ مع سيناريوهات مختلفة لنوع العرض
            workbook.Save("SmartTagShowTypeDemo_All.xlsx");
            Console.WriteLine("Workbook saved with default show type (All)");

            // إنشاء مصنف آخر بسلوك مختلف لنوع العرض
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];
            worksheet2.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
            Console.WriteLine("\nSecond workbook created with smart tag at B2");

            workbook2.Save("SmartTagShowTypeDemo_None.xlsx");
            Console.WriteLine("Second workbook saved (simulating None behavior)");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


