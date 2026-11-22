---
title: "الفئة GridExportTableOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.GridDesktop.Data.GridExportTableOptions الفئة. يمثل جميع خيارات تصدير الجدول"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridexporttableoptions/
---
## GridExportTableOptions class

يمثل جميع خيارات تصدير الجدول.

```csharp
public class GridExportTableOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridExportTableOptions](gridexporttableoptions/)() | منشئ GridExportTableOptions |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CheckMixedValueType](../../aspose.cells.griddesktop.data/gridexporttableoptions/checkmixedvaluetype/) { get; set; } | False، سيقوم Aspose.Cells بتعيين نوع DataColumn بناءً على نوع القيمة في الصف الأول للأداء. True، سيتحقق Aspose.Cells مما إذا كان نوع القيمة في العمود مختلطًا قبل تعيين نوع DataColumn، وإذا كان نوع القيمة مختلطًا، سيكون نوع DataColumn هو string. |
| [DataTable](../../aspose.cells.griddesktop.data/gridexporttableoptions/datatable/) { get; set; } | يحصل ويضبط DataTable الذي يتم تعيين نوع بيانات الأعمدة فيه. |
| [ExportAsHtmlString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportashtmlstring/) { get; set; } | يصدّر قيمة سلسلة HTML للخلايا إلى DataTable. |
| [ExportAsString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportasstring/) { get; set; } | يصدّر قيمة السلسلة للخلايا إلى DataTable. |
| [ExportColumnName](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportcolumnname/) { get; set; } | يشير إلى ما إذا كانت البيانات في الصف الأول تُصدّر إلى اسم العمود في DataTable. القيمة الافتراضية هي false. |
| [FormatStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/formatstrategy/) { get; set; } | يحصل ويضبط استراتيجية التنسيق عند تصدير القيمة كقيمة سلسلة. |
| [Indexes](../../aspose.cells.griddesktop.data/gridexporttableoptions/indexes/) { get; set; } | فهارس الأعمدة/الصفوف التي يجب تصديرها. |
| [IsVertical](../../aspose.cells.griddesktop.data/gridexporttableoptions/isvertical/) { get; set; } | True إذا كان الصف في ملف Workbook يمثل صفًا في DataTable. False إذا كان العمود في ملف Workbook يمثل صفًا في DataTable. |
| [PlotVisibleCells](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecells/) { get; set; } | يصدّر فقط الخلايا المرئية. |
| [PlotVisibleColumns](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecolumns/) { get; set; } | يصدّر فقط الأعمدة المرئية. |
| [PlotVisibleRows](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblerows/) { get; set; } | يصدّر فقط الصفوف المرئية. |
| [RenameStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/renamestrategy/) { get; set; } | استراتيجية لأسماء الأعمدة المكررة. |
| [SkipErrorValue](../../aspose.cells.griddesktop.data/gridexporttableoptions/skiperrorvalue/) { get; set; } | يشير إلى ما إذا كان يتم تخطي القيمة غير الصالحة للعمود. على سبيل المثال، إذا كان نوع العمود decimal والقيمة أكبر من decimal.MaxValue وهذه الخاصية true، لن نرمي استثناءً مرة أخرى. القيمة الافتراضية هي false. |

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


