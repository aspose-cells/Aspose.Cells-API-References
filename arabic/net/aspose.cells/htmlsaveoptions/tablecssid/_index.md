---
title: "HtmlSaveOptions.TableCssId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. يحصل ويضبط بادئة اسم css من النوع مثل trcoltd وما إلى ذلك، وهي موجودة في عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. القيمة الافتراضية هي"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/tablecssid/
---
## HtmlSaveOptions.TableCssId property

يحصل ويعيّن بادئة اسم نوع CSS مثل tr, col, td وغيرها، والتي تُضمّن في عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. القيمة الافتراضية هي "".

```csharp
public string TableCssId { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyTableCssIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // تكوين خيارات حفظ HTML باستخدام TableCssId
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.TableCssId = "custom-table-style";
            
            // حفظ دفتر العمل مع خيارات HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with TableCssId: " + saveOptions.TableCssId);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


