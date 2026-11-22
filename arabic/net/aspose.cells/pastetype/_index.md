---
title: "Enum PasteType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.PasteType enum. يمثل نوع اللصق الخاص"
type: docs
url: /ar/net/aspose.cells/pastetype/
---
## PasteType enumeration

يمثل نوع اللصق الخاص.

```csharp
public enum PasteType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| All | `0` | ينسخ جميع بيانات النطاق. |
| Default | `1` | يعمل كسلوك "All" في برنامج MS Excel. |
| AllExceptBorders | `2` | ينسخ جميع بيانات النطاق بدون النطاق. |
| DefaultExceptBorders | `3` | يعمل كسلوك "All except borders" في برنامج MS Excel. |
| ColumnWidths | `4` | ينسخ فقط عرض النطاق. |
| RowHeights | `5` | ينسخ فقط ارتفاع النطاق. |
| Comments | `6` | ينسخ فقط التعليقات في النطاق. |
| Formats | `7` | ينسخ فقط التنسيقات في النطاق. |
| Formulas | `8` | يقوم بنسخ الصيغ فقط في النطاق. |
| FormulasAndNumberFormats | `9` | يقوم بنسخ الصيغ وتنسيقات الأرقام فقط في النطاق. |
| Validation | `10` | يقوم بنسخ التحققات فقط في النطاق. |
| Values | `11` | يقوم بنسخ القيم فقط في النطاق. |
| ValuesAndFormats | `12` | يقوم بنسخ القيم والتنسيقات فقط في النطاق. |
| ValuesAndNumberFormats | `13` | يقوم بنسخ القيم وتنسيقات الأرقام فقط في النطاق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteTypeDemo
    {
        public static void PasteTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // حدد النطاق المصدر
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B4");

            // حدد النطاق الوجهة
            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange("D1:E4");

            // أنشئ PasteOptions واضبط PasteType
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                IgnoreLinksToOriginalFile = true
            };

            // انسخ النطاق المصدر إلى النطاق الوجهة باستخدام خيارات اللصق المحددة
            destinationRange.Copy(sourceRange, pasteOptions);

            // احفظ المصنف
            workbook.Save("PasteTypeExample.xlsx");

            // أخرج النتائج
            Console.WriteLine("Data copied with PasteType.Values and saved to PasteTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


