---
title: "تعداد SensitivityLabelMarkType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Metas.SensitivityLabelMarkType. يمثل أنواع وضع العلامات على المحتوى التي يجب تطبيقها على ملف"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabelmarktype/
---
## SensitivityLabelMarkType enumeration

يمثل أنواع وضع العلامات على المحتوى التي يجب تطبيقها على ملف.

```csharp
[Flags]
public enum SensitivityLabelMarkType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لا شيء |
| Header | `1` | رأس الصفحة |
| Footer | `2` | تذييل الصفحة |
| Watermark | `4` | علامة مائية |
| Encryption | `8` | تشفير |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelMarkTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض قيم تعداد SensitivityLabelMarkType
            SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;

            // تطبيق علامات تصنيف حساسية مختلفة بناءً على النوع
            switch (markType)
            {
                case SensitivityLabelMarkType.None:
                    Console.WriteLine("No sensitivity label applied");
                    break;
                case SensitivityLabelMarkType.Header:
                    worksheet.PageSetup.SetHeader(0, "CONFIDENTIAL");
                    break;
                case SensitivityLabelMarkType.Footer:
                    worksheet.PageSetup.SetFooter(0, "INTERNAL USE ONLY");
                    break;
                case SensitivityLabelMarkType.Watermark:
                    worksheet.PageSetup.SetHeader(0, "&KFF0000&DRAFT");
                    break;
                case SensitivityLabelMarkType.Encryption:
                    workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
                    break;
            }

            // حفظ المصنف مع تطبيق تصنيف الحساسية
            workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


