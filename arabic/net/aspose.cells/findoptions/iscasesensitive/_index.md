---
title: "FindOptions.IsCaseSensitive"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. تشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف"
type: docs
url: /ar/net/aspose.cells/findoptions/iscasesensitive/
---
## FindOptions.IsCaseSensitive property

يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف.

```csharp
[Obsolete("Use FindOptions.CaseSensitive property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCaseSensitive { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية FindOptions.CaseSensitive. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2010. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyIsCaseSensitiveDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين بيانات عينة
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("AbC");

            FindOptions options = new FindOptions();
            options.IsCaseSensitive = true;
            
            // ابحث عن تطابق حساس لحالة الأحرف
            Cell cell = worksheet.Cells.Find("abc", null, options);
            
            Console.WriteLine("Case-sensitive search for 'abc' found at: " + 
                              (cell != null ? cell.Name : "No match"));
        }
    }
}
```

### انظر أيضًا

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


