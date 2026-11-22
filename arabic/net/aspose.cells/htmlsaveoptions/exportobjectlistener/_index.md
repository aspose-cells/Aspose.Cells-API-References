---
title: "HtmlSaveOptions.ExportObjectListener"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. يحصل أو يضبط ExportObjectListener لتصدير الكائنات"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

يحصل أو يضبط ExportObjectListener لتصدير الكائنات.

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية HtmlSaveOptions.IStreamProvider. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2015. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportObjectListenerDemo
    {
        public static void Run()
        {
            // إنشاء مستمع تصدير كائن مخصص
            var listener = new CustomExportObjectListener();
            
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Export Object Listener");
            
            // إنشاء خيارات حفظ HTML مع المستمع
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = listener
            };

            // حفظ إلى ملف HTML
            workbook.Save("output.html", saveOptions);
        }
    }

    // تنفيذ مخصص لـ IExportObjectListener
    public class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // مثال: معالجة الكائن المُصدَّر
            Console.WriteLine($"Exporting object: {e.GetType()}");
            // إرجاع الكائن الأصلي (يمكن تعديله إذا لزم الأمر)
            return e;
        }
    }
}
```

### انظر أيضًا

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


