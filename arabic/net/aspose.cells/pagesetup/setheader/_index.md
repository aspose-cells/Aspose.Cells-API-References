---
title: "PageSetup.SetHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تعيين برنامج نصي لتنسيق رأس ملف Excel"
type: docs
url: /ar/net/aspose.cells/pagesetup/setheader/
---
## PageSetup.SetHeader method

يضبط تنسيق برنامج نصي لترويسة ملف Excel.

```csharp
public void SetHeader(int section, string headerScript)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| headerScript | String | نص تنسيق الرأس. |

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

على سبيل المثال: "&amp;Arial,Bold&amp;8Header Note"

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // قم بتعيين أقسام ترويسة مختلفة باستخدام أوامر متعددة
            pageSetup.SetHeader(0, "&F"); // Left section - File name
            pageSetup.SetHeader(1, "Page &P of &N"); // Center section - Page numbering
            pageSetup.SetHeader(2, "&D"); // Right section - Date

            workbook.Save("PageSetup_SetHeader_Example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


