---
title: "PageSetup.SetFooter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تقوم بتعيين برنامج نصي لتنسيق تذييل ملف Excel"
type: docs
url: /ar/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

يضبط تنسيق برنامج نصي لتذييل ملف Excel.

```csharp
public void SetFooter(int section, string footerScript)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| footerScript | String | نص تنسيق التذييل. |

### ملاحظات

أوامر النص البرمجي:

| **الأمر** | **الوصف** |
| --- | --- |
| &amp;P | رقم الصفحة الحالي |
| &amp;N | عدد الصفحات |
| &amp;D | التاريخ الحالي |
| &amp;T | الوقت الحالي |
| &amp;A | اسم الورقة |
| &amp;F | اسم الملف بدون المسار |
| &amp;\"&lt;FontName&gt;\" | اسم الخط، على سبيل المثال: &amp;\"Arial\" |
| &amp;\"&lt;FontName&gt;, &lt;FontStyle&gt;\" | اسم الخط ونمط الخط، على سبيل المثال: &amp;\"Arial,Bold\" |
| &amp;&lt;FontSize&gt; | حجم الخط. إذا تم اتباع هذا الأمر برقم عادي ليتم طباعته في الترويسة، فسيتم فصله عن ارتفاع الخط بمسافة حرفية. |
| &amp;K&lt;RRGGBB&gt; | لون الخط، على سبيل المثال (أحمر): &amp;KFF0000 |
| &amp;G | نص الصورة |

على سبيل المثال: "&amp;Arial,Bold&amp;8Footer Note"

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.SetFooter(0, "Page &P");
            worksheet.PageSetup.SetFooter(1, "&D");
            worksheet.PageSetup.SetFooter(2, "&A");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


