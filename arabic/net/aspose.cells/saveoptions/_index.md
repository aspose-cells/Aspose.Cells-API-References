---
title: "الفئة SaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.SaveOptions. تمثل جميع خيارات الحفظ"
type: docs
url: /ar/net/aspose.cells/saveoptions/
---
## SaveOptions class

يمثل جميع خيارات الحفظ

```csharp
public class SaveOptions
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | ما إذا كان سيتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عند إدخال قيمة أطول من 32 كيلوبايت، سيتم قطعها. |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | اجعل المصنف فارغًا بعد حفظ الملف. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | يشير إلى ما إذا كان سيتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | يشير إلى ما إذا كان سيتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | يشير إلى ما إذا كان سيتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | يحصل على تنسيق ملف الحفظ. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | يشير إلى ما إذا كان يتم تحديث إعداد Smart Art. القيمة الافتراضية هي false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | يحصل أو يضبط رد النداء التحذيري. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // إنشاء خيارات الحفظ - حفظ كملف CSV
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = ',';
            
            // إنشاء خيارات التحميل لملف CSV
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);

            // إعادة حفظ المصنف باستخدام الخيارات
            Workbook resavedWorkbook = Cells_Type_SaveOptions(workbook, saveOptions, loadOptions);

            // حفظ النتيجة إلى ملف
            resavedWorkbook.Save("output.csv", SaveFormat.Csv);
        }

        public static Workbook Cells_Type_SaveOptions(Workbook wb, SaveOptions optsSave, LoadOptions optsLoad)
        {
            using (MemoryStream ms = new MemoryStream(1048576))
            {
                wb.Save(ms, optsSave);
                ms.Position = 0;
                return new Workbook(ms, optsLoad);
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


