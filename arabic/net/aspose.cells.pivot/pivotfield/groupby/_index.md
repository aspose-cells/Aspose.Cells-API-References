---
title: "PivotField.GroupBy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تقوم بتجميع الحقل تلقائيًا بفاصل زمني"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_7}

تجميع الحقل تلقائيًا بفاصل زمني

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(double interval, bool newField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الفاصل | Double | القيمة الداخلية للمجموعة. سيتم تعيين قيمة تلقائية إذا كانت صفرًا، |
| newField | منطقي | تشير إلى ما إذا كان يتم إضافة حقل جديد إلى pivottable. فقط لمجموعة DateTime. |

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // إضافة حقل إلى منطقة العمود
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // تجميع الحقل بـ 1 (فاصل) بنطاق تلقائي
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_6}

تجميع الحقل تلقائيًا بالمعامل الداخلي

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المجموعات | PivotGroupByType[] | أنواع التجميع |
| الفاصل | Double | القيمة الداخلية للمجموعة. سيتم تعيين قيمة تلقائية إذا كانت صفرًا، تعمل فقط على التجميع حسب الأرقام أو الأيام. |
| newField | منطقي | تشير إلى ما إذا كان يتم إضافة حقل جديد إلى pivottable. |

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_5}

قم بتجميع الملف حسب أنواع مجموعات التاريخ.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| البداية | DateTime | وقت البدء datetime |
| النهاية | DateTime | نهاية datetime |
| المجموعات | PivotGroupByType[] | أنواع التجميع |
| الفاصل | Double | الفاصل الزمني |
| firstAsNewField | منطقي | يشير إلى ما إذا كان يتم إضافة حقل جديد إلى جدول المحور. فقط للعنصر الأول في المجموعة. |

### قيمة الإرجاع

يعني False أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة مع تواريخ لجدول المحور
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // احصل على حقل Pivot
            PivotField pivotField = pivotTable.RowFields[0];

            // جهّز المعلمات لطريقة GroupBy
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // استدعِ طريقة GroupBy مع معلمات التاريخ
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // تحديث جدول المحور
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_3}

قم بتجميع الملف حسب أنواع مجموعات التاريخ.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isAutoStart | منطقي | يشير إلى ما إذا كان سيتم الكشف تلقائيًا عن قيمة تاريخ ووقت البدء. |
| البداية | DateTime | وقت البدء datetime |
| isAutoEnd | منطقي | يشير إلى ما إذا كان سيتم الكشف تلقائيًا عن قيمة تاريخ ووقت النهاية. |
| النهاية | DateTime | نهاية datetime |
| المجموعات | PivotGroupByType[] | أنواع التجميع |
| الفاصل | Double | الفاصل الزمني |
| firstAsNewField | منطقي | يشير إلى ما إذا كان يتم إضافة حقل جديد إلى جدول المحور. فقط للعنصر الأول في المجموعة. |

### قيمة الإرجاع

يعني False أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_4}

قم بتجميع الملف حسب الرقم.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(double start, double end, double interval, bool newField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| البداية | Double | قيمة البدء |
| النهاية | Double | قيمة النهاية |
| الفاصل | Double | الفاصل الزمني |
| newField | منطقي | يشير إلى ما إذا كان يتم إضافة حقل جديد إلى جدول المحور |

### قيمة الإرجاع

يعني False أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // أضف حقل صف وقم بتجميعه
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // احفظ المصنف
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_2}

قم بتجميع الملف حسب الرقم.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isAutoStart | منطقي | يشير إلى ما إذا كان سيتم الكشف تلقائيًا عن قيمة البدء. |
| البداية | Double | قيمة البدء |
| isAutoEnd | منطقي | يشير إلى ما إذا كان سيتم الكشف تلقائيًا عن قيمة النهاية. |
| النهاية | Double | قيمة النهاية |
| الفاصل | Double | الفاصل الزمني |
| newField | منطقي | يشير إلى ما إذا كان يتم إضافة حقل جديد إلى جدول المحور |

### قيمة الإرجاع

يعني False أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

قم بتجميع الحقل مخصصًا.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | عناصر المجموعة المخصصة. |
| newField | منطقي | يشير إلى ما إذا كان يتم إضافة حقل جديد إلى جدول المحور |

### قيمة الإرجاع

يعني False أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions options) مع الخاصية PivotFieldGroupOptions.DiscreteGroupItems. سيتم إزالة هذه الطريقة بعد 6 أشهر منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // احصل على حقل Pivot
            PivotField pivotField = pivotTable.RowFields[0];

            // إنشاء عناصر مجموعة مخصصة
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // استدعاء طريقة GroupBy مع عناصر مجموعة مخصصة
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // تحديث جدول المحور
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DiscreteGroupItem[], bool) {#groupby_1}

قم بتجميع الحقل مخصصًا.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DiscreteGroupItem[] customGroupItems, bool newField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| customGroupItems | DiscreteGroupItem[] | عناصر المجموعة المخصصة. |
| newField | منطقي | يشير إلى ما إذا كان يتم إضافة حقل جديد إلى جدول المحور |

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions options) مع الخاصية PivotFieldGroupOptions.DiscreteGroupItems. سيتم إزالة هذه الطريقة بعد 6 أشهر منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* class [DiscreteGroupItem](../../discretegroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


