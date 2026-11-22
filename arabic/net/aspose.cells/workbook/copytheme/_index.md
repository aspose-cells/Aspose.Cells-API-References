---
title: "Workbook.CopyTheme"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تنسخ السمة من مصنف آخر"
type: docs
url: /ar/net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

ينسخ السمة من مصنف آخر.

```csharp
public void CopyTheme(Workbook source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | المصنف | مصنف المصدر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyThemeWithWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء مصنف المصدر (يتم تعيين السمة تلقائيًا عند فتح ملف القالب)
            Workbook sourceWorkbook = new Workbook(FileFormatType.Xlsx);

            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            
            // نسخ السمة من المصنف المصدر إلى المصنف الهدف
            destWorkbook.CopyTheme(sourceWorkbook);

            // حفظ دفتر العمل الوجهة
            destWorkbook.Save("output_with_theme.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


