---
title: "الفئة ExportTableOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ExportTableOptions. تمثل جميع خيارات تصدير الجدول"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/
---
## ExportTableOptions class

يمثل جميع خيارات تصدير الجدول.

```csharp
public class ExportTableOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ExportTableOptions](exporttableoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllowDBNull](../../aspose.cells/exporttableoptions/allowdbnull/) { get; set; } | تشير هذه القيمة إلى ما إذا كان مسموحًا بـ DBNulls في هذا الجدول. |
| [CheckMixedValueType](../../aspose.cells/exporttableoptions/checkmixedvaluetype/) { get; set; } | False، سيقوم Aspose.Cells بتعيين نوع DataColumn بناءً على نوع القيمة في الصف الأول للأداء. True، سيتحقق Aspose.Cells مما إذا كان نوع القيمة في العمود مختلطًا قبل تعيين نوع DataColumn، وإذا كان نوع القيمة مختلطًا، سيكون نوع DataColumn هو string. |
| [DataTable](../../aspose.cells/exporttableoptions/datatable/) { get; set; } | يحصل ويضبط DataTable الذي يتم تعيين نوع بيانات الأعمدة فيه. |
| [ExportAsHtmlString](../../aspose.cells/exporttableoptions/exportashtmlstring/) { get; set; } | يصدّر قيمة سلسلة HTML للخلايا إلى DataTable. |
| [ExportAsString](../../aspose.cells/exporttableoptions/exportasstring/) { get; set; } | يصدّر قيمة السلسلة للخلايا إلى DataTable. |
| [ExportColumnName](../../aspose.cells/exporttableoptions/exportcolumnname/) { get; set; } | يشير إلى ما إذا كانت البيانات في الصف الأول تُصدّر إلى اسم العمود في DataTable. القيمة الافتراضية هي false. |
| [FormatStrategy](../../aspose.cells/exporttableoptions/formatstrategy/) { get; set; } | يحصل ويضبط استراتيجية التنسيق عند تصدير القيمة كقيمة سلسلة. |
| [Indexes](../../aspose.cells/exporttableoptions/indexes/) { get; set; } | فهارس الأعمدة/الصفوف التي يجب تصديرها. |
| [IsVertical](../../aspose.cells/exporttableoptions/isvertical/) { get; set; } | True إذا كان الصف في ملف Workbook يمثل صفًا في DataTable. False إذا كان العمود في ملف Workbook يمثل صفًا في DataTable. |
| [PlotVisibleCells](../../aspose.cells/exporttableoptions/plotvisiblecells/) { get; set; } | يصدّر فقط الخلايا المرئية. |
| [PlotVisibleColumns](../../aspose.cells/exporttableoptions/plotvisiblecolumns/) { get; set; } | يصدّر فقط الأعمدة المرئية. |
| [PlotVisibleRows](../../aspose.cells/exporttableoptions/plotvisiblerows/) { get; set; } | يصدّر فقط الصفوف المرئية. |
| [RenameStrategy](../../aspose.cells/exporttableoptions/renamestrategy/) { get; set; } | استراتيجية لأسماء الأعمدة المكررة. |
| [SkipErrorValue](../../aspose.cells/exporttableoptions/skiperrorvalue/) { get; set; } | يشير إلى ما إذا كان يتم تخطي القيمة غير الصالحة للعمود. على سبيل المثال، إذا كان نوع العمود decimal والقيمة أكبر من decimal.MaxValue وهذه الخاصية true، لن نرمي استثناءً مرة أخرى. القيمة الافتراضية هي false. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [PreprocessExportedValue](../../aspose.cells/exporttableoptions/preprocessexportedvalue/)(int, int, CellValue) | معالجة مسبقة لقيمة الخلية الحالية لتصديرها. |

### ملاحظات

إذا كانت هناك بعض المتطلبات الخاصة بشأن التصدير، مثل تجاهل قيم الأخطاء، قد يقوم المستخدم بتمديد هذه الفئة لتجاوز واجهات برمجة التطبيقات المقابلة لتحقيق الهدف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ExportTableOptionsDemo
    {
        public static void ExportTableOptionsExample()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells[0, 0].PutValue("Name");
            worksheet.Cells[0, 1].PutValue("Age");
            worksheet.Cells[1, 0].PutValue("John");
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue("Jane");
            worksheet.Cells[2, 1].PutValue(25);

            // إنشاء مثال من ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                SkipErrorValue = true,
                PlotVisibleCells = true,
                PlotVisibleRows = true,
                PlotVisibleColumns = true,
                ExportAsString = false,
                ExportAsHtmlString = false,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                CheckMixedValueType = true,
                AllowDBNull = true,
                IsVertical = true,
                RenameStrategy = RenameStrategy.Digit
            };

            // تصدير البيانات من ورقة العمل إلى DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // عرض البيانات المصدرة
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // احفظ المصنف
            workbook.Save("ExportTableOptionsExample.xlsx");
            workbook.Save("ExportTableOptionsExample.pdf");
        }
    }

}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


