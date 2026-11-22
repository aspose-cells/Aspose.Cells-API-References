---
title: "TxtSaveOptions.KeepSeparatorsForBlankRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtSaveOptions. تشير إلى ما إذا كان يجب إخراج الفواصل للصف الفارغ. القيمة الافتراضية هي false لذا سيكون محتوى الصف الفارغ فارغًا"
type: docs
url: /ar/net/aspose.cells/txtsaveoptions/keepseparatorsforblankrow/
---
## TxtSaveOptions.KeepSeparatorsForBlankRow property

يشير إلى ما إذا كان يجب إخراج الفواصل للصف الفارغ. القيمة الافتراضية هي false، وبالتالي سيكون محتوى الصف الفارغ فارغًا.

```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyKeepSeparatorsForBlankRowDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // إضافة بعض البيانات مع صفوف فارغة
            cells[0, 0].PutValue("a");
            cells[0, 1].PutValue("b");
            cells[3, 0].PutValue("c");
            cells[4, 1].PutValue("d");

            // إنشاء خيارات حفظ مع تعيين KeepSeparatorsForBlankRow إلى true
            TxtSaveOptions options = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                KeepSeparatorsForBlankRow = true
            };

            // احفظ المصنف إلى CSV مع الخيارات
            string csvOutput = SaveAsCsv(wb, options);
            Console.WriteLine(csvOutput);
        }

        private static string SaveAsCsv(Workbook wb, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                wb.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
        }
    }
}
```

### انظر أيضًا

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


