---
title: "FindOptions.LookAtType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. انظر إلى النوع"
type: docs
url: /ar/net/aspose.cells/findoptions/lookattype/
---
## FindOptions.LookAtType property

انظر إلى النوع.

```csharp
public LookAtType LookAtType { get; set; }
```

### ملاحظات

عندما يكون [`RegexKey`](../regexkey/) صحيحًا ويكون المستخدم قد حدد القاعدة الدقيقة للتعبير النمطي، لأسباب تتعلق بالأداء يجب ضبط هذه الخاصية إلى EntireContent. وإلا سنعيد هيكلة مفتاح البحث لضمان إمكانية مطابقته وفق النوع المحدد. على سبيل المثال، عندما يكون النوع هو Contains (وهذه هي القيمة الافتراضية لهذه الخاصية)، سنضيف أحرفًا بدلية في بداية ونهاية مفتاح البحث تلقائيًا. في هذه الحالة، ستصبح التعبيرات النمطية أكثر تعقيدًا وستنخفض الأداء أيضًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookAtTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا وأضف بعض البيانات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("=1+2"); // Formula
            worksheet.Cells["A3"].PutValue("Partial match test");
            worksheet.Cells["A4"].PutValue("=A1&A3"); // Formula concatenating cells

            // أنشئ خيارات البحث مع LookAtType.EntireContent
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.EntireContent
            };

            // ابحث عن صيغة تتطابق تمامًا مع "=A1&A3"
            Cell cell = worksheet.Cells.Find("=A1&A3", null, options);
            Console.WriteLine("Found cell with exact formula match: " + (cell != null ? cell.Name : "null"));

            // غيّر إلى مطابقة جزئية
            options.LookAtType = LookAtType.Contains;
            cell = worksheet.Cells.Find("A3", null, options);
            Console.WriteLine("Found cell containing 'A3' in formula: " + (cell != null ? cell.Name : "null"));
        }
    }
}
```

### انظر أيضًا

* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


