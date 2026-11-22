---
title: "TxtLoadOptions.HeaderRowsCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. عدد صفوف الرأس التي سيتم تكرارها للأوراق الموسَّعة"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/headerrowscount/
---
## TxtLoadOptions.HeaderRowsCount property

عدد صفوف الرأس التي سيتم تكرارها للأوراق الموسعة.

```csharp
public int HeaderRowsCount { get; set; }
```

### ملاحظات

صفوف الرأس المحددة بهذه الخاصية ستُكرر لتلك الأوراق الموسَّعة. هذه الخاصية سَتعمل فقط عندما يكون [`ExtendToNextSheet`](../extendtonextsheet/) true.

### أمثلة

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderRowsCountDemo
    {
        public static void Run()
        {
            // إنشاء محتوى CSV نموذجي
            string csvData = "Header1,Header2,Header3\n" +
                            "Value1,Value2,Value3\n" +
                            "Value4,Value5,Value6\n" +
                            "Value7,Value8,Value9";

            // أنشئ TxtLoadOptions مع تعيين HeaderRowsCount إلى 1
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderRowsCount = 1
            };

            // حمّل بيانات CSV إلى دفتر عمل
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);

                // الوصول إلى ورقة العمل الأولى
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // أظهر أن الصف الأول يُعامل كرأس
                Console.WriteLine("Header Row:");
                for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                {
                    Console.Write(cells[0, col].StringValue + "\t");
                }
                Console.WriteLine("\n");

                // اعرض صفوف البيانات (متجاوزًا الرأس)
                Console.WriteLine("Data Rows:");
                for (int row = 1; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
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


