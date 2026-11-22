---
title: "PivotTableFormatCollection.FormatArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "PivotTableFormatCollection طريقة. يقوم بتنسيق المنطقة المحددة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
## PivotTableFormatCollection.FormatArea method

يقوم بتنسيق المنطقة المحددة.

```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition, 
    PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow, 
    bool isGrandColumn, Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| axisType | PivotFieldType | المنطقة في PivotTable التي ينطبق عليها هذه القاعدة. |
| fieldPosition | Int32 | موضع الحقل داخل المحور الذي تنطبق عليه هذه القاعدة. |
| subtotalType | PivotFieldSubtotalType | نوع مرشح المجموع الفرعي لحقل المحور |
| selectionType | PivotTableSelectionType | يشير إلى كيفية اختيار البيانات. |
| isGrandRow | منطقي | يشير إلى ما إذا كان يتم اختيار صفوف الإجمالي الكلي. |
| isGrandColumn | منطقي | يشير إلى ما إذا كان يتم اختيار أعمدة الإجمالي الكلي. |
| النمط | النمط | النمط الذي يطبق على منطقة جدول المحور. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionMethodFormatAreaWithPivotFieldTypeInt32PivotFieldSDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى PivotTable
            PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
            
            // إنشاء نمط للتنسيق
            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.LightGray;
            style.BackgroundColor = Color.LightGray;

            // تنسيق منطقة جدول المحور
            pt.PivotFormats.FormatArea(
                PivotFieldType.Row, 
                0, 
                PivotFieldSubtotalType.Automatic, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


