---
title: "الفئة PasteOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.PasteOptions. تمثل خيارات اللصق الخاصة"
type: docs
url: /ar/net/aspose.cells/pasteoptions/
---
## PasteOptions class

يمثل خيارات اللصق الخاص.

```csharp
public class PasteOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PasteOptions](pasteoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IgnoreLinksToOriginalFile](../../aspose.cells/pasteoptions/ignorelinkstooriginalfile/) { get; set; } | تجاهل الروابط إلى الملف الأصلي. |
| [KeepOldTables](../../aspose.cells/pasteoptions/keepoldtables/) { get; set; } | يحافظ على الجداول في النطاق الوجهة. |
| [OnlyVisibleCells](../../aspose.cells/pasteoptions/onlyvisiblecells/) { get; set; } | True يعني نسخ الخلايا المرئية فقط. |
| [OperationType](../../aspose.cells/pasteoptions/operationtype/) { get; set; } | يحصل على ويضبط نوع العملية عند لصق النطاق. |
| [PasteType](../../aspose.cells/pasteoptions/pastetype/) { get; set; } | نوع اللصق الخاص. |
| [ShiftFormulasOfShapes](../../aspose.cells/pasteoptions/shiftformulasofshapes/) { get; set; } | يشير إلى ما إذا كان يجب إزاحة صيغ الأشكال عند نسخ النطاقات. |
| [SkipBlanks](../../aspose.cells/pasteoptions/skipblanks/) { get; set; } | يشير إلى ما إذا كان يتخطى الخلايا الفارغة. |
| [Transpose](../../aspose.cells/pasteoptions/transpose/) { get; set; } | True لعكس الصفوف والأعمدة عند لصق النطاق. القيمة الافتراضية هي False. |

### أمثلة

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsDemo
    {
        public static void PasteOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات إلى ورقة العمل الأولى
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // أنشئ ورقة عمل أخرى
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");

            // حدد النطاق المصدر
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1:A3");

            // حدد النطاق الوجهة
            Aspose.Cells.Range destRange = sheet2.Cells.CreateRange("B1:B3");

            // أنشئ كائن PasteOptions
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = true
            };

            // انسخ النطاق باستخدام خيارات اللصق المحددة
            destRange.Copy(sourceRange, pasteOptions);

            // احفظ المصنف
            workbook.Save("PasteOptionsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


