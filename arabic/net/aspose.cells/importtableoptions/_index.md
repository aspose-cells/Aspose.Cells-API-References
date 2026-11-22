---
title: "الفئة ImportTableOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ImportTableOptions الفئة. تمثل خيارات استيراد البيانات إلى الخلايا"
type: docs
url: /ar/net/aspose.cells/importtableoptions/
---
## ImportTableOptions class

يمثل خيارات استيراد البيانات إلى الخلايا.

```csharp
public class ImportTableOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ImportTableOptions](importtableoptions/)() | ينشئ خيارات الاستيراد الافتراضية. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CheckMergedCells](../../aspose.cells/importtableoptions/checkmergedcells/) { get; set; } | يشير إلى ما إذا كان يتم فحص الخلايا المدمجة. |
| [ColumnIndexes](../../aspose.cells/importtableoptions/columnindexes/) { get; set; } | يحصل أو يضبط الأعمدة (بدءًا من الصفر) للاستيراد من مصدر البيانات. يعني null أنه يجب استيراد جميع الأعمدة. |
| [ConvertGridStyle](../../aspose.cells/importtableoptions/convertgridstyle/) { get; set; } | يشير إلى ما إذا كان يتم تطبيق نمط عرض الشبكة على الخلايا. |
| [ConvertNumericData](../../aspose.cells/importtableoptions/convertnumericdata/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب تحويل القيمة النصية إلى قيمة رقمية أو تاريخية. |
| [DateFormat](../../aspose.cells/importtableoptions/dateformat/) { get; set; } | يحصل أو يضبط سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيم تاريخ ووقت مستوردة. |
| [DefaultValues](../../aspose.cells/importtableoptions/defaultvalues/) { get; set; } | القيمة الافتراضية للقيمة في الجدول هي null. |
| [ExportCaptionAsFieldName](../../aspose.cells/importtableoptions/exportcaptionasfieldname/) { get; set; } | يشير إلى ما إذا كان يتم تصدير العنوان كاسم الحقل |
| [InsertRows](../../aspose.cells/importtableoptions/insertrows/) { get; set; } | يشير إلى ما إذا كان يجب إضافة صفوف جديدة لاستيراد سجلات البيانات. |
| [IsFieldNameShown](../../aspose.cells/importtableoptions/isfieldnameshown/) { get; set; } | يشير إلى ما إذا كان يجب استيراد اسم الحقل. |
| [IsFormulas](../../aspose.cells/importtableoptions/isformulas/) { get; set; } | يشير إلى ما إذا كانت البيانات صيغًا. |
| [IsHtmlString](../../aspose.cells/importtableoptions/ishtmlstring/) { get; set; } | يشير إلى ما إذا كانت القيمة تحتوي على وسوم HTML. |
| [NumberFormats](../../aspose.cells/importtableoptions/numberformats/) { get; set; } | يحصل أو يضبط تنسيقات الأرقام |
| [ShiftFirstRowDown](../../aspose.cells/importtableoptions/shiftfirstrowdown/) { get; set; } | يشير إلى ما إذا كان يتم إزاحة الصف الأول إلى الأسفل عند إدراج الصفوف. |
| [Styles](../../aspose.cells/importtableoptions/styles/) { get; set; } | يحصل ويضبط الأنماط لكل عمود في الجدول. |
| [TotalColumns](../../aspose.cells/importtableoptions/totalcolumns/) { get; set; } | يحصل أو يضبط العدد الإجمالي للأعمدة للاستيراد من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |
| [TotalRows](../../aspose.cells/importtableoptions/totalrows/) { get; set; } | يحصل أو يضبط العدد الإجمالي للصفوف للاستيراد من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsDemo
    {
        public static void ImportTableOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ DataTable للاستيراد
            DataTable dataTable = new DataTable("SampleData");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Date", typeof(DateTime));
            dataTable.Rows.Add(1, "John Doe", DateTime.Now);
            dataTable.Rows.Add(2, "Jane Smith", DateTime.Now.AddDays(1));

            // أنشئ مثيلًا من ImportTableOptions
            ImportTableOptions importOptions = new ImportTableOptions
            {
                ConvertGridStyle = true,
                ConvertNumericData = true,
                InsertRows = true,
                ShiftFirstRowDown = false,
                IsFieldNameShown = true,
                ExportCaptionAsFieldName = false,
                DateFormat = "yyyy-MM-dd",
                TotalRows = -1, // Import all rows
                TotalColumns = -1, // Import all columns
                IsHtmlString = false,
                CheckMergedCells = false
            };

            // استيراد DataTable إلى ورقة العمل
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // احفظ المصنف
            workbook.Save("ImportTableOptionsExample.xlsx");
            workbook.Save("ImportTableOptionsExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


