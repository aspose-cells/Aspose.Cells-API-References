---
title: "DbfSaveOptions.ExportAsString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DbfSaveOptions. تشير إلى ما إذا كان التصدير كقيمة نصية"
type: docs
url: /ar/net/aspose.cells.saving/dbfsaveoptions/exportasstring/
---
## DbfSaveOptions.ExportAsString property

يحدد ما إذا كان التصدير كقيمة نصية

```csharp
public bool ExportAsString { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة بأنواع مختلطة
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("TextValue");

            // إنشاء مثيل DbfSaveOptions
            DbfSaveOptions options = new DbfSaveOptions();

            // عرض قيمة ExportAsString الحالية
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // تعيين ExportAsString إلى true (جميع القيم سيتم تصديرها كنصوص)
            options.ExportAsString = true;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // حفظ مع ExportAsString = true
            workbook.Save("ExportAsStringTrue.dbf", options);

            // تعيين ExportAsString إلى false (القيم ستحافظ على أنواعها الأصلية)
            options.ExportAsString = false;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // حفظ مع ExportAsString = false
            workbook.Save("ExportAsStringFalse.dbf", options);
        }
    }
}
```

### انظر أيضًا

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


