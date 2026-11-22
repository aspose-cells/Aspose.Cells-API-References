---
title: "TxtLoadOptions.HeaderColumnsCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. عدد أعمدة الرأس التي سيتم تكرارها للأوراق الموسعة"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/headercolumnscount/
---
## TxtLoadOptions.HeaderColumnsCount property

عدد أعمدة الرأس التي سيتم تكرارها للأوراق الموسعة.

```csharp
public int HeaderColumnsCount { get; set; }
```

### ملاحظات

أعمدة الرأس المحددة بهذه الخاصية ستتكرر لتلك الأوراق الموسعة. هذه الخاصية لا تعمل إلا عندما تكون [`ExtendToNextSheet`](../extendtonextsheet/) صحيحة.

### أمثلة

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderColumnsCountDemo
    {
        public static void Run()
        {
            // إنشاء محتوى CSV نموذجي
            string csvData = "Header1,Header2,Header3,Data1,Data2,Data3\n" +
                            "H1,H2,H3,D1,D2,D3\n" +
                            "A,B,C,D,E,F\n" +
                            "G,H,I,J,K,L";

            // إنشاء TxtLoadOptions مع تعيين HeaderColumnsCount إلى 3
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderColumnsCount = 3, // First 3 columns will be treated as headers
                Encoding = Encoding.UTF8
            };

            // حمّل بيانات CSV إلى دفتر عمل
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // عرض أعمدة الرأس (الأعمدة الثلاثة الأولى)
                Console.WriteLine("Header Columns:");
                for (int row = 0; row < 2; row++)
                {
                    for (int col = 0; col < options.HeaderColumnsCount; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // عرض أعمدة البيانات (الأعمدة المتبقية)
                Console.WriteLine("\nData Columns:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = options.HeaderColumnsCount; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


