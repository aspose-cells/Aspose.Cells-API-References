---
title: "HtmlSaveOptions.ExportCellCoordinate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم تصدير إحداثيات إكسل للخلايا غير الفارغة عند حفظ الملف إلى html. القيمة الافتراضية هي false. إذا كنت تريد استيراد html الناتج إلى إكسل يرجى الحفاظ على القيمة الافتراضية"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportcellcoordinate/
---
## HtmlSaveOptions.ExportCellCoordinate property

تشير إلى ما إذا كان يتم تصدير إحداثيات Excel للخلايا غير الفارغة عند حفظ الملف إلى html. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

```csharp
public bool ExportCellCoordinate { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCellCoordinateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // إنشاء خيارات حفظ HTML وتمكين ExportCellCoordinate
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportCellCoordinate = true;

            // احفظ دفتر العمل كـ HTML مع إحداثيات الخلايا
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with cell coordinates exported successfully.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


