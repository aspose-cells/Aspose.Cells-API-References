---
title: "SheetRender.ToTiff"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SheetRender. عرض كامل worksheet كصورة Tiff إلى الدفق"
type: docs
url: /ar/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

عرض كامل ورقة العمل كصورة Tiff إلى تدفق.

```csharp
public void ToTiff(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | تدفق الصورة الناتجة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToTiffWithStreamDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف محتوى نموذجي لتوضيح العرض
            worksheet.Cells["A1"].PutValue("Aspose.Cells TIFF Rendering Demo");
            
            // قم بتكوين خيارات الصورة للعرض
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // أنشئ مُعالج ورقة مع الخيارات المكوَّنة
            SheetRender renderer = new SheetRender(worksheet, options);
            try
            {
                // أنشئ دفق إخراج لصورة TIFF
                using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
                {
                    // اعرض worksheet إلى TIFF باستخدام الدفق
                    renderer.ToTiff(tiffStream);
                    Console.WriteLine("Worksheet successfully rendered to TIFF stream.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during TIFF rendering: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

عرض كامل ورقة العمل كصورة Tiff إلى ملف.

```csharp
public void ToTiff(string filename)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الملف | String | اسم ملف الصورة الناتجة |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToTiffWithStringDemo
    {
        public static void Run()
        {
            // تحميل ملف Excel المصدر.
            Workbook workbook = new Workbook("Book1.xlsx");

            // إنشاء خيارات الصورة أو الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.SaveFormat = SaveFormat.Tiff;

            // إنشاء عرض ورقة للورقة الأولى.
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);

            // احفظ جميع صفحات الورقة كملف TIFF متعدد الصفحات
            sheetRender.ToTiff("output.tiff");
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


