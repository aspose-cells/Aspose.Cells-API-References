---
title: "ReferredArea.StartColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReferredArea. العمود الأول للمنطقة"
type: docs
url: /ar/net/aspose.cells/referredarea/startcolumn/
---
## ReferredArea.StartColumn property

عمود البداية للمنطقة.

```csharp
public int StartColumn { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["C1"].PutValue("Cherry");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);

            // إنشاء نطاق مسمى يشير إلى B1:C2
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!B1:C2";

            // الحصول على المنطقة المشار إليها مع تعيين إعادة الحساب إلى false
            ReferredArea referredArea = name.GetReferredAreas(false)[0];

            // عرض خاصية StartColumn
            Console.WriteLine("Start Column: " + referredArea.StartColumn);
            Console.WriteLine("End Column: " + referredArea.EndColumn);

            // طباعة القيم في المنطقة المشار إليها باستخدام StartColumn
            Cells cells = worksheet.Cells;
            for (int row = referredArea.StartRow; row <= referredArea.EndRow; row++)
            {
                for (int col = referredArea.StartColumn; col <= referredArea.EndColumn; col++)
                {
                    Console.WriteLine(cells[row, col].Name + ": " + cells[row, col].Value);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


