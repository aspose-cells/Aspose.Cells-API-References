---
title: "ImageOrPrintOptions.WarningCallback"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تعيين رد نداء التحذير"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/warningcallback/
---
## ImageOrPrintOptions.WarningCallback property

يحصل أو يضبط رد النداء التحذيري.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة محتوى سيتسبب في توليد تحذير أثناء التصيير
            worksheet.Cells["A1"].PutValue("This text uses a non-existent font");
            Style style = workbook.CreateStyle();
            style.Font.Name = "NonExistentFont";
            worksheet.Cells["A1"].SetStyle(style);

            // أنشئ مثيلًا لـ ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // عرض القيمة الأولية لـ WarningCallback
            Console.WriteLine("Current WarningCallback value: " + options.WarningCallback);

            // إنشاء وتعيين رد نداء تحذير مخصص
            var warningCallback = new RenderingWarningCallback();
            options.WarningCallback = warningCallback;

            // إنشاء SheetRender لعرض رد نداء أثناء التصيير
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_image.png");

            // تحقق مما إذا تم التقاط التحذيرات
            Console.WriteLine($"Total warnings captured: {warningCallback.WarningCount}");
        }
    }

    // تنفيذ رد نداء مخصص لمعالجة تحذيرات التصيير
    public class RenderingWarningCallback : IWarningCallback
    {
        public int WarningCount { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            // معالجة تحذيرات استبدال الخطوط
            if (warningInfo.WarningType == WarningType.FontSubstitution)
            {
                Console.WriteLine($"Font substitution warning: {warningInfo.Description}");
                WarningCount++;
            }
        }
    }
}
```

### انظر أيضًا

* interface [IWarningCallback](../../../aspose.cells/iwarningcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


