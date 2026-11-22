---
title: "PivotTable.CalculateData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تحسب بيانات جدول المحور إلى الخلايا"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata_1}

يحسب بيانات جدول المحور إلى الخلايا.

```csharp
public void CalculateData()
```

### ملاحظات

هذه الطريقة تحسب البيانات فقط باستخدام البيانات المخزنة مؤقتًا في [`PivotCache`](../pivotcache/). لذا إذا كنت تريد الحساب باستخدام مصدر البيانات الأحدث، يرجى استخدام طريقة [`Refresh`](../../pivotcache/refresh/) للحساب. إذا تم تغيير إعدادات جدول المحور فقط، فإن `CalculateData` يكفي.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            
            DateTime baseDate = new DateTime(2021, 11, 1);
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+2}"].PutValue(baseDate.AddDays(i));
                worksheet.Cells[$"B{i+2}"].PutValue(100 + i * 10);
            }

            // إنشاء جدول محوري - تم الإصلاح عن طريق ضمان المعلمات الصحيحة
            int pivotIndex = worksheet.PivotTables.Add("A1:B16", "D3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // أضف حقولًا إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // تطبيق مرشح التاريخ
            PivotField dateField = pivotTable.RowFields[0];
            dateField.FilterByDate(PivotFilterType.November, new DateTime(2021, 1, 1), new DateTime(2021, 12, 31));
            
            // احسب بيانات الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata}

يحسب جدول المحور مع الخيارات.

```csharp
public PivotTable[] CalculateData(PivotTableCalculateOption option)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيار | PivotTableCalculateOption | الخيارات لحساب جدول المحور |

### قيمة الإرجاع

يعيد جميع جداول المحور التي تم حسابها. إذا كان [`RefreshData`](../../pivottablecalculateoption/refreshdata/) صحيحًا، سيتم حساب جميع جداول المحور المستندة إلى نفس ذاكرة التخزين المؤقت للجدول المحوري معًا.

### ملاحظات

إذا كان [`RefreshData`](../../pivottablecalculateoption/refreshdata/) صحيحًا، ستقوم هذه الطريقة بتحديث ذاكرة التخزين المؤقت للجدول المحوري من مصدر البيانات، ثم حساب جميع جداول المحور بناءً على نفس ذاكرة التخزين المؤقت. وإلا، سيتم الحساب فقط باستخدام البيانات المخزنة مؤقتًا في ذاكرة التخزين المؤقت.

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataWithPivotTableCalculateOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // عيّن خيارات الحساب
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // احسب باستخدام الخيارات
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


