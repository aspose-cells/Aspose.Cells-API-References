---
title: "HorizontalPageBreakCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HorizontalPageBreakCollection. تحصل على عنصر HorizontalPageBreak عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

يحصل على العنصر [`HorizontalPageBreak`](../../horizontalpagebreak/) عند الفهرس المحدد.

```csharp
public HorizontalPageBreak this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف فواصل صفحات أفقية
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            // الوصول إلى فواصل الصفحات باستخدام خاصية Item
            HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
            Console.WriteLine("First page break row: " + firstBreak.Row);
            
            // تعديل الخلايا التي تؤثر على فواصل الصفحات
            worksheet.Cells.DeleteRows(0, 2);
            
            // تحقق من تعديل فاصل الصفحة
            Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### انظر أيضًا

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

يحصل على العنصر [`HorizontalPageBreak`](../../horizontalpagebreak/) بالاسم المحدد للخلية.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
```

| معامل | الوصف |
| --- | --- |
| cellName | اسم الخلية. |

### قيمة الإرجاع

العنصر بالاسم المحدد للخلية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class HorizontalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف عددًا من فواصل الصفحات الأفقية باستخدام تحميلات مختلفة
                worksheet.HorizontalPageBreaks.Add(5);          // break after row index 5
                worksheet.HorizontalPageBreaks.Add("D5");      // break at cell D5 (row index 4)

                // ----- الوصول عبر فهرس عدد صحيح (Item[int]) -----
                // خاصية Item هي الفهرس، لذا نستخدم صيغة []
                HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
                Console.WriteLine("First break row (int index): " + firstBreak.Row);

                // ----- الوصول عبر مفتاح نصي (Item[string]) -----
                // استرجع فاصل الصفحة الذي تم إضافته باستخدام اسم الخلية "D5"
                HorizontalPageBreak breakByCell = worksheet.HorizontalPageBreaks["D5"];
                Console.WriteLine("Break added with \"D5\" is at row: " + breakByCell.Row);

                // احفظ المصنف للتحقق من بقاء فواصل الصفحات
                workbook.Save("HorizontalPageBreaks_ItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


