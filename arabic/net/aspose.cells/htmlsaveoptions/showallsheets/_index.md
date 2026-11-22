---
title: "HtmlSaveOptions.ShowAllSheets"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم إظهار جميع الأوراق عند الحفظ كملف html واحد"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/showallsheets/
---
## HtmlSaveOptions.ShowAllSheets property

يشير إلى ما إذا كان سيتم عرض جميع الأوراق عند الحفظ كملف html واحد.

```csharp
public bool ShowAllSheets { get; set; }
```

### ملاحظات

يعمل فقط عندما يكون [`SaveAsSingleFile`](../saveassinglefile/) صحيحًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyShowAllSheetsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد يحتوي على عدة أوراق
            Workbook workbook = new Workbook();
            
            // إضافة بيانات إلى الورقة الأولى
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            sheet1.Cells["A1"].PutValue("Sheet 1 Content");

            // إضافة ورقة ثانية
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            sheet2.Cells["B2"].PutValue("Sheet 2 Content");

            // إضافة ورقة ثالثة
            Worksheet sheet3 = workbook.Worksheets.Add("ThirdSheet");
            sheet3.Cells["C3"].PutValue("Sheet 3 Content");

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // تعيين خاصية ShowAllSheets إلى true لتصدير جميع الأوراق
            saveOptions.ShowAllSheets = true;

            // حفظ المصنف مع إظهار جميع الأوراق في HTML
            workbook.Save("ShowAllSheetsDemo.html", saveOptions);

            Console.WriteLine("HTML file with all sheets exported successfully.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


