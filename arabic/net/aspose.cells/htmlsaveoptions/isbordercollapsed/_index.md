---
title: "HtmlSaveOptions.IsBorderCollapsed"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كانت حدود الجدول مضغوطة. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/isbordercollapsed/
---
## HtmlSaveOptions.IsBorderCollapsed property

يشير إلى ما إذا كانت حدود الجدول مدمجة. القيمة الافتراضية هي true.

```csharp
public bool IsBorderCollapsed { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsBorderCollapsedDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية وحدود
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("With Borders");
            worksheet.Cells["B2"].SetStyle(style);

            // تعيين الثقافة للعرض
            var culture = new System.Globalization.CultureInfo("de-DE");
            Thread.CurrentThread.CurrentCulture = culture;
            Thread.CurrentThread.CurrentUICulture = culture;
            workbook.Settings.CultureInfo = culture;

            // إنشاء خيارات حفظ HTML وتعيين IsBorderCollapsed
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.IsBorderCollapsed = false;

            // حفظ دفتر العمل مع خيارات HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "HtmlWithBorders.html");
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("File saved with collapsed borders: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


