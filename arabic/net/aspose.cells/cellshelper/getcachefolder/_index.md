---
title: "CellsHelper.GetCacheFolder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تحصل على المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت"
type: docs
url: /ar/net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

يحصل على المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

```csharp
public static string GetCacheFolder()
```

### قيمة الإرجاع

المجلد لملفات التخزين المؤقت التي تم تحديدها. إذا لم يتم تحديده، سيتم إرجاع null وسيُستخدم مسار النظام المؤقت عند الحاجة.

### ملاحظات

تُستخدم ملفات الذاكرة المؤقتة عادةً لبعض الميزات المتعلقة بأداء الذاكرة، مثل حفظ مجموعة بيانات كبيرة إلى ملف xls، أو استخدام وضع الذاكرة مع تخزين مؤقت للملفات لنموذج الخلايا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetCacheFolderDemo
    {
        public static void Run()
        {
            try
            {
                // احصل على مسار مجلد التخزين المؤقت الحالي
                string cacheFolder = CellsHelper.GetCacheFolder();

                // عرض مسار مجلد التخزين المؤقت
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // اختياريًا تحديد مجلد تخزين مؤقت جديد (لتوضيح الطريقة المرتبطة)
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // تحقق من التغيير
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // العودة إلى الأصل (اختياري)
                CellsHelper.SetCacheFolder(cacheFolder);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with cache folder: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


