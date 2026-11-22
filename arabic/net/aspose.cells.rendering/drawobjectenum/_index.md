---
title: "تعداد DrawObjectEnum"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Rendering.DrawObjectEnum. يشير إلى خلية أو صورة لكائن DrawObject"
type: docs
url: /ar/net/aspose.cells.rendering/drawobjectenum/
---
## DrawObjectEnum enumeration

الإشارة إلى خلية أو صورة من DrawObject.

```csharp
public enum DrawObjectEnum
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Image | `0` | يشير إلى أن DrawObject هو صورة |
| Cell | `1` | يشير إلى أن DrawObject هو خلية |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassDrawObjectEnumDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وإضافة بيانات نموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Cell");

            // إنشاء كائن PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // إنشاء DrawObjectEventHandler مخصص
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            // حفظ المصنف كملف PDF باستخدام المعالج المخصص
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // تحقق مما إذا كان كائن الرسم خلية
            if (drawObject.Type == DrawObjectEnum.Cell)
            {
                Cell cell = drawObject.Cell;
                
                // إخراج معلومات الخلية
                Console.WriteLine($"Drawing Cell - Row: {cell.Row}, Column: {cell.Column}");
                Console.WriteLine($"Position: ({x}, {y}), Size: {width}x{height}");
                
                // معالجة خاصة للخلية A1
                if (cell.Row == 0 && cell.Column == 0)
                {
                    Console.WriteLine("This is cell A1");
                }
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


