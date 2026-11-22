---
title: "ReferredArea.IsEntireRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReferredArea. تشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الأعمدة أو الصف الكامل"
type: docs
url: /ar/net/aspose.cells/referredarea/isentirerow/
---
## ReferredArea.IsEntireRow property

يشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الأعمدة (صف كامل).

```csharp
public bool IsEntireRow { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // إنشاء نطاق مسمى يشير إلى الصف الكامل 2
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$2:$2";

            // احصل على المنطقة المشار إليها للنطاق المسمى
            ReferredArea referredArea = workbook.Worksheets.Names["NamedRange1"].GetReferredAreas(false)[0];

            // عرض القيمة الحالية لـ IsEntireRow
            Console.WriteLine("IsEntireRow value for NamedRange1: " + referredArea.IsEntireRow);

            // إنشاء نطاق مسمى آخر يشير إلى نطاق محدد (ليس صفًا كاملًا)
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // احصل على المنطقة المشار إليها للنطاق المسمى الثاني
            ReferredArea referredArea2 = workbook.Worksheets.Names["NamedRange2"].GetReferredAreas(false)[0];

            // عرض القيمة الحالية لـ IsEntireRow للنطاق الثاني
            Console.WriteLine("IsEntireRow value for NamedRange2: " + referredArea2.IsEntireRow);

            // توضيح تأثير IsEntireRow عن طريق فحص أبعاد النطاق
            Console.WriteLine("NamedRange1 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("NamedRange2 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // احفظ المصنف
            workbook.Save("ReferredAreaPropertyIsEntireRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


