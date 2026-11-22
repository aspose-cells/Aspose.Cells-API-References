---
title: "PptxSaveOptions.PptxSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ PptxSaveOptions. يمثل خيارات حفظ pptx"
type: docs
url: /ar/net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

يمثل خيارات حفظ pptx.

```csharp
public PptxSaveOptions()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Visible Data");
            worksheet.Cells["A2"].PutValue("Hidden Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // إخفاء الصف الثاني
            worksheet.Cells.Rows[1].IsHidden = true;

            // إنشاء PptxSaveOptions باستخدام المنشئ
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;

            // حفظ المصنف إلى PPTX مع الخيارات
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved to PPTX with hidden rows ignored.");
        }
    }
}
```

### انظر أيضًا

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

تمثل خيارات حفظ ملف .pptx.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| saveAsImage | منطقي | إذا كان True، سيتم تحويل المصنف إلى بعض الصور في ملف .pptx. إذا كان False، سيتم تحويل المصنف إلى بعض الجداول في ملف .pptx. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using System;

    public class PptxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            try
            {
                // استدعاء طريقة #ctor مع معامل منطقي
                bool saveAsImage = true;
                PptxSaveOptions options = new PptxSaveOptions(saveAsImage);

                // عيّن الخصائص الإضافية
                options.IgnoreHiddenRows = true;
                options.ExportViewType = SlideViewType.View;

                // حفظ المصنف باستخدام خيارات PPTX
                workbook.Save("PptxSaveOptionsCtorDemo.pptx", options);

                Console.WriteLine("PptxSaveOptions constructor executed successfully with parameter: " + saveAsImage);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PptxSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


