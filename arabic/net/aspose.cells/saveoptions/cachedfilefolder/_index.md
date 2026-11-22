---
title: "SaveOptions.CachedFileFolder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات"
type: docs
url: /ar/net/aspose.cells/saveoptions/cachedfilefolder/
---
## SaveOptions.CachedFileFolder property

المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

```csharp
public string CachedFileFolder { get; set; }
```

### ملاحظات

إذا لم يتم تحديد المجلد، فإن القيمة الافتراضية له هي [`GetCacheFolder`](../../cellshelper/getcachefolder/). إذا كانت القيمة الافتراضية null أو فارغة، أو تم تحديدها كـ null أو فارغة، فلن يتم استخدام أي ملف تخزين مؤقت عند حفظ دفتر العمل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCachedFileFolderDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test cached file folder");

            // تعيين خيارات الحفظ مع مجلد الملفات المخزنة مؤقتًا
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.CachedFileFolder = "TempCache"; // Specify cache folder

            // احفظ المصنف
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with cached file folder option.");
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


