---
title: "الفئة XlsbSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.XlsbSaveOptions فئة. يمثل الخيارات لحفظ ملف xlsb"
type: docs
url: /ar/net/aspose.cells/xlsbsaveoptions/
---
## XlsbSaveOptions class

يمثل الخيارات لحفظ ملف xlsb.

```csharp
public class XlsbSaveOptions : SaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [XlsbSaveOptions](xlsbsaveoptions/#constructor)() | ينشئ خيارات حفظ ملف xlsb. |
| [XlsbSaveOptions](xlsbsaveoptions/#constructor_1)(SaveFormat) | (**مهمل.**) ينشئ خيارات حفظ ملف xlsb. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة مؤقتة للبيانات. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K، سيتم قطعها. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | اجعل دفتر العمل فارغًا بعد حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CompressionType](../../aspose.cells/xlsbsaveoptions/compressiontype/) { get; set; } | يحصل أو يضبط نوع الضغط لملف ooxml. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ExportAllColumnIndexes](../../aspose.cells/xlsbsaveoptions/exportallcolumnindexes/) { get; set; } | يشير إلى ما إذا كان يتم تصدير جميع فهارس الأعمدة للخلايا. |
| [LightCellsDataProvider](../../aspose.cells/xlsbsaveoptions/lightcellsdataprovider/) { get; set; } | مزود البيانات لحفظ المصنف في الوضع الخفيف. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | يشير إلى ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | يحصل على تنسيق حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | يحصل أو يعيّن رد الاتصال التحذيري.(موروث من [`SaveOptions`](../saveoptions/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsbSaveOptionsDemo
    {
        public static void XlsbSaveOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // إنشاء مثيل من XlsbSaveOptions
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                CompressionType = OoxmlCompressionType.Level6,
                ExportAllColumnIndexes = true,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // احفظ المصنف كملف XLSB باستخدام الخيارات المحددة
            workbook.Save("XlsbSaveOptionsExample.xlsb", saveOptions);

            return;
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


