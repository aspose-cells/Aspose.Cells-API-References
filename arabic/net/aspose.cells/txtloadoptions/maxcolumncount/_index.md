---
title: "TxtLoadOptions.MaxColumnCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. الحد الأقصى لعدد الأعمدة التي سيتم استيرادها لورقة واحدة"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

الحد الأقصى لعدد الأعمدة التي سيتم استيرادها لورقة واحدة.

```csharp
public int MaxColumnCount { get; set; }
```

### ملاحظات

الأعمدة التي تتجاوز هذا الحد سيتم تجاهلها أو تمديدها إلى الورقة التالية وفقًا لـ [`ExtendToNextSheet`](../extendtonextsheet/). هذا العدد يشمل أعمدة الرأس ([`HeaderColumnsCount`](../headercolumnscount/)). القيمة القصوى هي حد الأعمدة لتنسيق الملف المقابل، مثل ملف xlsx حيث يكون 16384. إذا لم يتم تحديد هذه الخاصية أو كانت القيمة المحددة غير موجبة، فسيتم استخدام الحد الأقصى أيضًا.

### أمثلة

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxColumnCountDemo
    {
        public static void Run()
        {
            // إنشاء محتوى CSV نموذجي
            string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
                            "1,2,3,4,5,6,7,8,9,10,11\n" +
                            "a,b,c,d,e,f,g,h,i,j,k";

            // إنشاء TxtLoadOptions مع تعيين MaxColumnCount إلى 5
            TxtLoadOptions options = new TxtLoadOptions
            {
                MaxColumnCount = 5  // Only load first 5 columns
            };

            // تحميل ملف CSV بأعمدة محدودة
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // إخراج البيانات المحملة (يجب أن تكون الأعمدة الخمسة الأولى فقط موجودة)
                Console.WriteLine("Data loaded with MaxColumnCount = 5:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // تحقق من أنه تم تحميل 5 أعمدة فقط
                Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
            }
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


