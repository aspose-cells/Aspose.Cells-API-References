---
title: "الفئة ImageSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ImageSaveOptions. تمثل خيارات حفظ الصورة. للاستخدام المتقدم يرجى استخدام WorkbookRender أو SheetRender"
type: docs
url: /ar/net/aspose.cells/imagesaveoptions/
---
## ImageSaveOptions class

يمثل خيارات حفظ الصورة. للاستخدام المتقدم، يرجى استخدام [`WorkbookRender`](../../aspose.cells.rendering/workbookrender/) أو [`SheetRender`](../../aspose.cells.rendering/sheetrender/).

```csharp
public class ImageSaveOptions : SaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/#constructor)() | ينشئ الخيارات لحفظ ملف الصورة. |
| [ImageSaveOptions](imagesaveoptions/#constructor_1)(SaveFormat) | ينشئ الخيارات لحفظ ملف الصورة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة مؤقتة للبيانات. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K، سيتم قطعها. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | اجعل دفتر العمل فارغًا بعد حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ImageOrPrintOptions](../../aspose.cells/imagesaveoptions/imageorprintoptions/) { get; } | خيارات إضافية لإنشاء الصورة. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | يشير إلى ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | يحصل على تنسيق حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [StreamProvider](../../aspose.cells/imagesaveoptions/streamprovider/) { get; set; } | يحصل أو يعيّن IStreamProvider لتصدير الكائنات. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | يحصل أو يعيّن رد الاتصال التحذيري.(موروث من [`SaveOptions`](../saveoptions/).) |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassImageSaveOptionsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Image Export");

            // تعيين مسار الوجهة
            string destPath = "output.png";

            // إنشاء خيارات حفظ الصورة
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            
            // تخصيص خيارات الحفظ
            saveOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            saveOptions.ImageOrPrintOptions.OnlyArea = true;

            // حفظ دفتر العمل مع خيارات الصورة
            workbook.Save(destPath, saveOptions);

            Console.WriteLine("Image saved successfully to: " + destPath);
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


