---
title: "PivotTable.RefreshData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تُحدّث البيانات من مصدرها إلى ذاكرة التخزين المؤقت للجدول المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

يُحدّث البيانات من مصدرها إلى ذاكرة التخزين المؤقت للجدول المحوري.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData()
```

### ملاحظات

سنقوم بجمع البيانات من مصدر البيانات إلى مخزن مؤقت للبيفوت، ثم حساب البيانات في المخزن إلى الخلايا. ومن الأفضل أن يمكنك ببساطة استدعاء [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) لتحديث وحساب جميع جداول البيفوت في الملف، بدلاً من تحديث كل واحدة على حدة. ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة [`Refresh`](../../pivotcache/refresh/) وإزالة [`CalculateData`](../calculatedata/) المتبعة لأن جدول البيفوت هذا سيُحسب عند تحديث [`PivotCache`](../pivotcache/). ستُزال هذه الطريقة بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة صفوف وحقول بيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // تحديث وحساب بيانات جدول البيفوت
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // احفظ المصنف
            workbook.Save("PivotTableRefreshDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

يقوم بتحديث بيانات جدول البيفوت وإعداداته من مصدر البيانات مع الخيارات.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيار | PivotTableRefreshOption | الخيارات لتحديث مصدر بيانات جدول PivotTable. |

### ملاحظات

سنقوم بجمع البيانات من مصدر البيانات إلى مخزن مؤقت للبيفوت، ثم حساب البيانات في المخزن إلى الخلايا. ومن الأفضل أن يمكنك ببساطة استدعاء [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) لتحديث وحساب جميع جداول البيفوت في الملف، بدلاً من تحديث كل واحدة على حدة. ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة [`Refresh`](../../pivotcache/refresh/) وإزالة [`CalculateData`](../calculatedata/) المتبعة لأن جدول البيفوت هذا سيُحسب عند تحديث [`PivotCache`](../pivotcache/). ستُزال هذه الطريقة بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل التي تحتوي على جدول البيفوت
            Worksheet worksheet = workbook.Worksheets["PNL_AFS"];
            
            // الحصول على أول جدول بيفوت في ورقة العمل
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // تكوين خيارات التحديث
            PivotTableRefreshOption refreshOptions = new PivotTableRefreshOption();
            refreshOptions.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // تحديث بيانات جدول البيفوت باستخدام الخيارات المحددة
            pivotTable.RefreshData(refreshOptions);
            pivotTable.CalculateData();
            
            // احفظ المصنف المعدل
            workbook.Save("example_modified.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


