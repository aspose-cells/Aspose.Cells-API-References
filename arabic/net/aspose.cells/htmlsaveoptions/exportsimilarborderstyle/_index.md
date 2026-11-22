---
title: "HtmlSaveOptions.ExportSimilarBorderStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان سيتم تصدير نمط الحدود المتشابه عندما لا يدعم المتصفحات نمط الحدود. إذا كنت تريد استيراد ملف html أو mht إلى Excel يرجى الحفاظ على القيمة الافتراضية. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportsimilarborderstyle/
---
## HtmlSaveOptions.ExportSimilarBorderStyle property

تشير إلى ما إذا كان يتم تصدير نمط الحدود المشابه عندما لا يدعم المتصفحات نمط الحدود. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. القيمة الافتراضية هي false.

```csharp
public bool ExportSimilarBorderStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSimilarBorderStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات تجريبية مع حدود
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["B1"].PutValue("Similar Border");
            worksheet.Cells["B1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["C1"].PutValue("Different Border");
            worksheet.Cells["C1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Thin));

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                ExportSimilarBorderStyle = true // Demonstrate the property
            };

            // احفظ المصنف
            workbook.Save("output.html", htmlSaveOptions);
        }

        private static Style CreateBorderStyle(Workbook workbook, CellBorderType borderType)
        {
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = borderType;
            style.Borders[BorderType.BottomBorder].LineStyle = borderType;
            style.Borders[BorderType.LeftBorder].LineStyle = borderType;
            style.Borders[BorderType.RightBorder].LineStyle = borderType;
            return style;
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


