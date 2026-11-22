---
title: "PivotField.ShowValuesAs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تعرض قيم حقل البيانات بتنسيق عرض مختلف عندما يكون حساب ShowDataAs قيد الاستخدام"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

يعرض قيم حقل البيانات بتنسيق عرض مختلف عندما يكون حساب ShowDataAs قيد الاستخدام.

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | نوع تنسيق عرض البيانات. |
| baseField | Int32 | الفهرس إلى الحقل الذي تستند إليه عملية حساب ShowDataAs. |
| baseItemPositionType | PivotItemPositionType | نوع الموضع للعنصر الأساسي. |
| baseItem | Int32 | الفهرس إلى العنصر الأساسي الذي تستند إليه عملية حساب ShowDataAs. يعمل فقط عندما تكون baseItemPositionType مخصصة. |

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن قديمة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2026. تقدم Aspose اعتذارها عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Quarter");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue(1500);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Q1");
            worksheet.Cells["C4"].PutValue(800);
            
            worksheet.Cells["A5"].PutValue("Furniture");
            worksheet.Cells["B5"].PutValue("Q2");
            worksheet.Cells["C5"].PutValue(1200);

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // إضافة حقل الصف
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // إضافة حقل عمود
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // إضافة حقل بيانات وتكوين ShowValuesAs
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // احسب البيانات واحفظها
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

يحدد حساب \"إظهار القيم كـ\" لهذا الحقل المحوري.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | نوع عملية حساب "Show Values As". |
| baseField | Int32 | فهرس الحقل الأساسي المستخدم في العملية الحسابية. |
| baseItem | Int32 | فهرس العنصر الأساسي للعملية الحسابية. استخدم [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1) للعنصر السابق، [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) للعنصر التالي؛ القيم غير السالبة تشير إلى الفهرس الترتيبي لعنصر محور معين. |

### ملاحظات

للحقل البيانات فقط.

### انظر أيضًا

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

يضبط حساب \"إظهار القيم كـ\" لهذا حقل البيانات.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | نوع العملية الحسابية لـ Show Values As. |
| baseField | String | اسم الحقل الأساسي المستخدم في العملية الحسابية. |
| baseItem | String | تسمية عنصر محور عادي. يقبل أيضًا الكلمات المفتاحية المحجوزة: `(previous)` للعنصر السابق، `(next)` للعنصر التالي. مرّر `null` إذا كان نوع العملية الحسابية المحدد لا يتطلب عنصرًا أساسيًا. |

### انظر أيضًا

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


