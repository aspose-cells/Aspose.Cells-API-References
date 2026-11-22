---
title: "الفئة DbfSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Saving.DbfSaveOptions. تمثل خيارات حفظ ملف dbf"
type: docs
url: /ar/net/aspose.cells.saving/dbfsaveoptions/
---
## DbfSaveOptions class

يمثل خيارات حفظ ملف dbf

```csharp
public class DbfSaveOptions : SaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DbfSaveOptions](dbfsaveoptions/)() | خيارات حفظ ملف .dbf. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. (موروثة من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K، سيتم قطعها. (موروثة من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | اجعل دفتر العمل فارغًا بعد حفظ الملف. (موروثة من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | إذا كانت true وكان الدليل غير موجود، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. (موروثة من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportAsString](../../aspose.cells.saving/dbfsaveoptions/exportasstring/) { get; set; } | يحدد ما إذا كان التصدير كقيمة نصية |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | يشير إلى ما إذا كان يجب تخزين أحدث بيانات المخطط في الذاكرة المؤقتة. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | يحصل على تنسيق ملف الحفظ. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | يشير إلى ما إذا كان يتم تحديث إعداد Smart Art. القيمة الافتراضية هي false. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | يحصل أو يعيّن رد الاتصال للتحذير. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassDbfSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء مثيل من DbfSaveOptions
            DbfSaveOptions saveOptions = new DbfSaveOptions();
            
            // تعيين الخاصية ExportAsString
            saveOptions.ExportAsString = true;

            // حفظ المصنف باستخدام خيارات حفظ DBF
            workbook.Save("output.dbf", saveOptions);

            Console.WriteLine("Workbook saved as DBF with ExportAsString set to true.");
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


