---
title: "LoadOptions.IgnoreNotPrinted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تجاهل البيانات التي لم تُطبع إذا تم طباعة الملف مباشرةً"
type: docs
url: /ar/net/aspose.cells/loadoptions/ignorenotprinted/
---
## LoadOptions.IgnoreNotPrinted property

تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً

```csharp
public bool IgnoreNotPrinted { get; set; }
```

### ملاحظات

فقط لملف xlsx.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreNotPrintedDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML وتعيين IgnoreNotPrinted
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.AutoFitColsAndRows = true;

            // تحميل ملف HTML باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("example.html", loadOptions);
            Worksheet worksheet = workbook.Worksheets[0];

            // إظهار تأثير IgnoreNotPrinted عن طريق فحص أنماط الخلايا
            Console.WriteLine("B3 Cell Color: " + worksheet.Cells["B3"].GetStyle().ForegroundColor);
            Console.WriteLine("B4 Cell Color: " + worksheet.Cells["B4"].GetStyle().ForegroundColor);
            Console.WriteLine("B5 Cell Color: " + worksheet.Cells["B5"].GetStyle().ForegroundColor);

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


