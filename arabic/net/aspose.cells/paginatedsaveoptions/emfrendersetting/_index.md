---
title: "PaginatedSaveOptions.EmfRenderSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. إعداد لتصيير ملف Emf التعريفي"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/emfrendersetting/
---
## PaginatedSaveOptions.EmfRenderSetting property

إعداد لتصوير ملف Emf الميتا.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### ملاحظات

ملفات تعريف EMF التي تم تحديدها كـ "EMF+ Dual" يمكن أن تحتوي على كل من سجلات EMF+ وسجلات EMF. يمكن استخدام أي نوع من السجلات لتصيير الصورة، أو سجلات EMF+ فقط، أو سجلات EMF فقط. عندما يتم تعيين EmfPlusPrefer، سيتم تحليل سجلات EMF+ أثناء التصيير إلى الصفحة، وإلا سيتم تحليل سجلات EMF فقط. القيمة الافتراضية هي EmfOnly.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            // إنشاء صورة لعرض EMF
            worksheet.Pictures.Add(10, 10, "example.png");

            // تكوين خيارات الحفظ باستخدام إعدادات EMF عبر PdfSaveOptions
            PdfSaveOptions options = new PdfSaveOptions()
            {
                EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
            };

            // احفظ دفتر العمل باستخدام إعدادات EMF
            workbook.Save("EmfRenderSettingDemo.pdf", options);
        }
    }
}
```

### انظر أيضًا

* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


