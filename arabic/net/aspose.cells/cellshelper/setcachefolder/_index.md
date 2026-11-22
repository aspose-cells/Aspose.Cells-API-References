---
title: "CellsHelper.SetCacheFolder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تحدد المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت"
type: docs
url: /ar/net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

يضبط المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

```csharp
public static void SetCacheFolder(string cache)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ذاكرة مؤقتة | String | مجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت. |

### ملاحظات

تُستخدم ملفات الذاكرة المؤقتة عادةً لبعض الميزات المتعلقة بأداء الذاكرة، مثل حفظ مجموعة بيانات كبيرة إلى ملف xls، أو استخدام وضع الذاكرة مع تخزين مؤقت للملفات لنموذج الخلايا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodSetCacheFolderWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دليل مؤقت للذاكرة المؤقتة
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // تحديد مجلد التخزين المؤقت باستخدام CellsHelper
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // تحقق من أن مجلد التخزين المؤقت تم تحديده
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // إنشاء دفتر عمل بسيط لتوضيح الوظيفة
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // احفظ المصنف
                workbook.Save("CacheFolderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with cache folder configured.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting cache folder: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


