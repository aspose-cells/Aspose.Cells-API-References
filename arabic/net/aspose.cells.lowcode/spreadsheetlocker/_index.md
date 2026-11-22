---
title: "فئة SpreadsheetLocker"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.LowCode.SpreadsheetLocker. واجهة برمجة تطبيقات منخفضة الكود لقفل ملف جدول البيانات"
type: docs
url: /ar/net/aspose.cells.lowcode/spreadsheetlocker/
---
## SpreadsheetLocker class

واجهة برمجة تطبيقات منخفضة الكود لقفل ملف جدول البيانات.

```csharp
public class SpreadsheetLocker
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | يقفل ملف جدول البيانات بالإعدادات المحددة. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | يقفل ملف جدول البيانات بالإعدادات المحددة. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | يقفل ملف جدول البيانات بالإعدادات المحددة. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | يقفل ملف جدول البيانات بالإعدادات المحددة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassSpreadsheetLockerDemo
    {
        public static void Run()
        {
            // استخدم SpreadsheetLocker لحماية المصنف
            SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


