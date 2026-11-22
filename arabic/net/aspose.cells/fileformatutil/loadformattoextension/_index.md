---
title: "FileFormatUtil.LoadFormatToExtension"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FileFormatUtil. تحول قيمة تعداد تنسيق التحميل إلى امتداد ملف"
type: docs
url: /ar/net/aspose.cells/fileformatutil/loadformattoextension/
---
## FileFormatUtil.LoadFormatToExtension method

يحول قيمة تعداد تنسيق التحميل إلى امتداد ملف.

```csharp
public static string LoadFormatToExtension(LoadFormat loadFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadFormat | LoadFormat | تنسيق الملف المحمّل. |

### قيمة الإرجاع

الامتداد المرجع هو سلسلة بحروف صغيرة مع نقطة في البداية.

### ملاحظات

إذا لم يمكن تحويله، تُعيد null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodLoadFormatToExtensionWithLoadFormatDemo
    {
        public static void Run()
        {
            // عرض LoadFormatToExtension مع قيم LoadFormat مختلفة
            Console.WriteLine("Auto format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Auto));
            Console.WriteLine("CSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Csv));
            Console.WriteLine("Excel97-2003 format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Excel97To2003));
            Console.WriteLine("XLSX format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsx));
            Console.WriteLine("TSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Tsv));
            Console.WriteLine("ODS format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Ods));
            Console.WriteLine("XLSB format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsb));
        }
    }
}
```

### انظر أيضًا

* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


