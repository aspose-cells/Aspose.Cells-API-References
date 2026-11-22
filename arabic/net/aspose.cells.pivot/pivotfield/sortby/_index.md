---
title: "PivotField.SortBy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تقوم بفرز هذا الحقل المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder) {#sortby}

يقوم بفرز هذا الحقل المحوري.

```csharp
public void SortBy(SortOrder sortType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sortType | SortOrder | نوع الفرز لهذا الحقل. |

### انظر أيضًا

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int) {#sortby_1}

يقوم بفرز هذا الحقل المحوري.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method or PivotField.IsAutoSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sortType | SortOrder | نوع الفرز لهذا الحقل. |
| fieldSortedBy | Int32 | فهرس الحقل المحوري الذي يتم الفرز بناءً عليه. -1 يعني الفرز حسب تسميات البيانات لهذا الحقل، والقيم الأخرى تعني فهرس حقل البيانات الذي يتم الفرز بناءً عليه. |

### ملاحظات

ملاحظة: هذه الخاصية الآن قديمة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.SortBy(SortOrder, int,string) أو خاصية PivotField.IsAutoSort بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("UK");
            worksheet.Cells["A4"].PutValue("Germany");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقل الصف
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // قم بفرز حقل الصف بترتيب تنازلي باستخدام الفهرس -1
            rowField.SortBy(SortOrder.Descending, -1);
            
            // تحديث وحساب الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_2}

يقوم بفرز هذا الحقل المحوري.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sortType | SortOrder | نوع الفرز لهذا الحقل. |
| fieldSortedBy | Int32 | فهرس الحقل المحوري الذي يتم الفرز بناءً عليه. -1 يعني الفرز حسب تسميات البيانات لهذا الحقل، والقيم الأخرى تعني فهرس حقل البيانات الذي يتم الفرز بناءً عليه. |
| dataType | PivotLineType | نوع البيانات التي يتم الفرز بناءً عليها. |
| cellName | String | فرز حسب القيم في الصف أو العمود |

### ملاحظات

ملاحظة: هذه الخاصية الآن قديمة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.SortBy(SortOrder, int,string) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("B");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);
            worksheet.Cells["B4"].PutValue(100);

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // فرز حقل الصف
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
            
            // حساب البيانات
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, string) {#sortby_3}

يقوم بفرز هذا الحقل المحوري.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sortType | SortOrder | نوع الفرز لهذا الحقل. |
| fieldSortedBy | Int32 | فهرس الحقل المحوري الذي يتم الفرز بناءً عليه. -1 يعني الفرز حسب تسميات البيانات لهذا الحقل، والقيم الأخرى تعني فهرس حقل البيانات الذي يتم الفرز بناءً عليه. |
| cellName | String | فرز حسب القيم في الصف أو العمود. إذا كان Null، يتم التجميع حسب إجمالي الحقل، وإلا يتم التجميع حسب القيم في العمود أو الصف المحدد. |

### انظر أيضًا

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


