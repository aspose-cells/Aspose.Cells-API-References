---
title: "فئة WorkbookDesigner"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.WorkbookDesigner. تغلف الكائن الذي يمثل جدول بيانات مصمم"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

يحتوي على الكائن الذي يمثل جدول بيانات المصمم.

```csharp
public class WorkbookDesigner
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | يُهيئ نسخة جديدة من الفئة `WorkbookDesigner`. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | يُهيئ نسخة جديدة من الفئة `WorkbookDesigner`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | يشير إلى ما إذا كان يجب حساب الصيغ. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | يحصل ويضبط واجهة الاستدعاء لمعالجة smartmarker. |
| [ContainsVariables](../../aspose.cells/workbookdesigner/containsvariables/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كانت ورقة العمل الأولى تحتوي على متغيرات مخصصة. |
| [EnableHeaderFooterMarkers](../../aspose.cells/workbookdesigner/enableheaderfootermarkers/) { get; set; } | يشير إلى ما إذا كان الرأس/التذييل يحتوي على علامات ذكية ويجب معالجتها معًا. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يتم معالجة العلامة الذكية سطرًا بسطر. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | يشير إلى ما إذا كانت الصيغ المتكررة مع صف المجموع الفرعي. |
| [SortDataSource](../../aspose.cells/workbookdesigner/sortdatasource/) { get; set; } | يشير إلى ما إذا كان يتم فرز مصدر البيانات. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | إذا كان TRUE، سيتم إدراج Null إذا كانت القيمة ""؛ |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | يشير إلى ما إذا كانت المراجع في أوراق عمل أخرى سيتم تحديثها. |
| [VariablesWorksheetName](../../aspose.cells/workbookdesigner/variablesworksheetname/) { get; set; } | يحصل ويضبط اسم ورقة العمل التي تحتوي على متغيرات smart marker. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | يحصل على ويضبط كائن [`Workbook`](./workbook/). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | يمسح جميع مصادر البيانات. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | يرجع مجموعة من العلامات الذكية في جدول بيانات. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | يعالج العلامات الذكية ويملأ قيم مصدر البيانات. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | يعالج العلامات الذكية ويملأ قيم مصدر البيانات. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | يعالج العلامات الذكية ويملأ قيم مصدر البيانات. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | (**Obsolete.**) يعالج العلامات الذكية ويملأ قيم مصدر البيانات. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | يضبط مصدر البيانات لكائن DataSet. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | يضبط مصدر البيانات لكائن DataTable. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | يضبط مصدر البيانات لكائن DataView. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | يضبط مصدر البيانات لكائن OleDbConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | يضبط مصدر البيانات لكائن SqlConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | يضبط مصدر البيانات لكائن DataView ويربطه باسم مصدر البيانات. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | يضبط مصدر البيانات لكائن [`ICellsDataTable`](../icellsdatatable/). |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | يضبط ربط البيانات إلى متغير. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | يضبط مصدر البيانات لكائن IDataReader. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) | تعيين قيمة سلسلة JSON كمصدر بيانات للعلامات الذكية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerDemo
    {
        public static void WorkbookDesignerExample()
        {
            // إنشاء كائن WorkbookDesigner
            WorkbookDesigner wd = new WorkbookDesigner();

            // فتح ملف القالب (الذي يحتوي على العلامات الذكية)
            wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");

            // تهيئة البيانات الخاصة بك من مصدر البيانات
            DataSet ds = new DataSet();
            // إضافة بيانات إلى مجموعة البيانات (هذا مجرد مثال، استبدله بمصدر البيانات الفعلي)
            DataTable dt = new DataTable("Table1");
            dt.Columns.Add("Column1");
            dt.Columns.Add("Column2");
            dt.Rows.Add("Value1", "Value2");
            dt.Rows.Add("Value11", "Value22");
            ds.Tables.Add(dt);

            // تعيين مجموعة البيانات كمصدر البيانات
            wd.SetDataSource(ds);

            // معالجة العلامات الذكية لملء البيانات في أوراق العمل
            wd.Process(true);

            // احفظ ملف Excel
            wd.Workbook.Save("WorkbookDesignerExample.xlsx");

            // عرض خصائص أخرى
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // مسح مصدر البيانات
            wd.ClearDataSource();

            // تعيين مصدر البيانات باستخدام طرق مختلفة
            wd.SetDataSource("dataSourceName", dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource("dataSourceName", new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
            wd.SetDataSource("variable", new object());

            // معالجة العلامات الذكية مرة أخرى
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // حفظ ملف Excel مرة أخرى
            wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


