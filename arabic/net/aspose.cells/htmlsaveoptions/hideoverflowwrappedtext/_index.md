---
title: "HtmlSaveOptions.HideOverflowWrappedText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "HtmlSaveOptions property. يشير إلى ما إذا كان يتم إخفاء النص المتجاوز عندما يتم تعيين تنسيق الخلية لتغليف النص. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

يشير إلى ما إذا كان سيتم إخفاء النص المتجاوز عندما يتم تعيين تنسيق الخلية إلى التفاف النص. القيمة الافتراضية هي false

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // حدد نصًا تجريبيًا في الخلية A1
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
            
            // إنشاء وتطبيق نمط مع تغليف النص
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // احصل على مجموعة الخلايا وطبق النمط
            Cells cells = worksheet.Cells;
            cells["A1"].SetStyle(style, flag);
            
            // حدد عرض العمود لجعل النص يلتف
            cells.SetColumnWidth(0, 10);
            
            // إنشاء خيارات حفظ HTML وتعيين HideOverflowWrappedText
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            
            // حفظ المصنف باستخدام خيارات HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


