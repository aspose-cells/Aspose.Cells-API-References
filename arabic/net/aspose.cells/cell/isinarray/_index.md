---
title: "Cell.IsInArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة"
type: docs
url: /ar/net/aspose.cells/cell/isinarray/
---
## Cell.IsInArray property

يشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة.

```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.IsArrayFormula للتحقق مما إذا كانت صيغة الخلية صيغة مصفوفة. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2018. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsInArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة بصيغ مصفوفة
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // تعيين صيغة مصفوفة باستخدام الواجهة البرمجية الصحيحة
            worksheet.Cells["C2"].SetArrayFormula("A2:A3*B2:B3", 2, 1);

            // التحقق من خاصية IsInArray
            Cell cellInArray = worksheet.Cells["C2"];
            Cell cellNotInArray = worksheet.Cells["A2"];

            Console.WriteLine("Cell C2 is in array: " + cellInArray.IsInArray);
            Console.WriteLine("Cell A2 is in array: " + cellNotInArray.IsInArray);

            // إظهار مسح الخلايا غير المصفوفة
            for (int row = 1; row <= 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = worksheet.Cells[row, col];
                    if (!cell.IsInArray && !cell.IsFormula)
                    {
                        cell.PutValue("");
                    }
                }
            }

            // احفظ المصنف
            workbook.Save("IsInArrayDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


