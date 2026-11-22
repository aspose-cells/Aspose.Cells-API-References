---
title: "تعداد SignatureType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.SignatureType. يحدد نوع التوقيع"
type: docs
url: /ar/net/aspose.cells.drawing/signaturetype/
---
## SignatureType enumeration

يحدد نوع التوقيع.

```csharp
public enum SignatureType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | القيمة الافتراضية، قيمة ProviderId المقابلة ثابتة إلى {0000000000-0000-0000-0000-0000000000}. |
| Stamp | `1` | قيمة ProviderId المقابلة عادةً هي {000CD6A4-0000-0000-C000-000000000046}. |
| Custom | `3` | عادةً ما تحتاج قيمة ProviderId المقابلة إلى أن يتم تعيينها من قبل المستخدم. يجب الحصول عليها من الوثائق المرفقة مع الموفر. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassSignatureTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة خطوط توقيع بأنواع مختلفة
            Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
            stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;

            Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
            customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
            customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");

            // حفظ دفتر العمل مع إعدادات التوقيع
            workbook.Save("SignatureTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


