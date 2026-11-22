---
title: "TxtSaveOptions.TrimTailingBlankCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtSaveOptions. تشير إلى ما إذا كان يجب قص الخلايا الفارغة المتتبقة في صف واحد. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/txtsaveoptions/trimtailingblankcells/
---
## TxtSaveOptions.TrimTailingBlankCells property

يشير إلى ما إذا كان يجب قص الخلايا الفارغة المتبقية في صف واحد. القيمة الافتراضية هي false.

```csharp
public bool TrimTailingBlankCells { get; set; }
```

### ملاحظات

عند الحفظ باستخدام وضع LightCells ولم يتم تحديد [`ExportArea`](../exportarea/)، لا يؤثر هذا الخيار وسيتم تمديد صف واحد إلى آخر خلية توفرها تنفيذية [`LightCellsDataProvider`](../lightcellsdataprovider/)

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimTailingBlankCellsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // أضف بيانات تجريبية
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[0, 2].PutValue("C");
            cells[1, 0].PutValue(1);
            cells[1, 2].PutValue(2);
            cells[2, 0].PutValue(3);

            // احفظ دون قص الخلايا الفارغة المتتبقة (الافتراضي)
            TxtSaveOptions options1 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = false
            };
            string result1 = SaveAsCsv(workbook, options1);
            Console.WriteLine("Without TrimTailingBlankCells:\n" + result1);

            // احفظ مع قص الخلايا الفارغة المتتبقة
            TxtSaveOptions options2 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = true
            };
            string result2 = SaveAsCsv(workbook, options2);
            Console.WriteLine("\nWith TrimTailingBlankCells:\n" + result2);
        }

        private static string SaveAsCsv(Workbook workbook, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                workbook.Save(stream, options);
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


