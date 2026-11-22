---
title: "EbookSaveOptions.EbookSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ EbookSaveOptions. ينشئ خيارات لحفظ ملف الكتاب الإلكتروني"
type: docs
url: /ar/net/aspose.cells.saving/ebooksaveoptions/ebooksaveoptions/
---
## EbookSaveOptions() {#constructor}

ينشئ خيارات لحفظ ملف الكتاب الإلكتروني.

```csharp
public EbookSaveOptions()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class EbookSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة محتوى تجريبي
            worksheet.Cells["A1"].PutValue("Ebook Test");
            worksheet.Cells["A2"].PutValue("This is a test for EbookSaveOptions");
            
            // إنشاء EbookSaveOptions باستخدام المنشئ
            EbookSaveOptions saveOptions = new EbookSaveOptions();
            
            // احفظ المصنف باستخدام EbookSaveOptions (يحفظ تلقائيًا كـ EPUB)
            workbook.Save("output.epub", saveOptions);
            
            Console.WriteLine("Ebook saved successfully with EbookSaveOptions constructor.");
        }
    }
}
```

### انظر أيضًا

* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)

---

## EbookSaveOptions(SaveFormat) {#constructor_1}

ينشئ خيارات لحفظ ملف الكتاب الإلكتروني.

```csharp
public EbookSaveOptions(SaveFormat saveFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| saveFormat | SaveFormat | تنسيق الملف. يجب أن يكون Epub أو Azw3. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Sample Ebook Content");
            
            try
            {
                // استدعاء طريقة #ctor مع معامل SaveFormat
                EbookSaveOptions saveOptions = new EbookSaveOptions(SaveFormat.Epub);
                
                // عيّن الخصائص الإضافية إذا لزم الأمر
                saveOptions.Encoding = System.Text.Encoding.UTF8;
                
                Console.WriteLine("EbookSaveOptions constructor executed successfully with SaveFormat.Epub");
                
                // حفظ المصنف باستخدام الخيارات التي تم إنشاؤها
                workbook.Save("EbookSaveOptionsDemo.epub", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


