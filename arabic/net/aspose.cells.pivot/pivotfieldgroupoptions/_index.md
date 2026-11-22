---
title: "الفئة PivotFieldGroupOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotFieldGroupOptions. خيارات إعدادات تجميع حقل المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldgroupoptions/
---
## PivotFieldGroupOptions class

خيارات إعدادات تجميع حقل محوري.

```csharp
public class PivotFieldGroupOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PivotFieldGroupOptions](pivotfieldgroupoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DiscreteGroupItems](../../aspose.cells.pivot/pivotfieldgroupoptions/discretegroupitems/) { get; set; } | يحصل ويضبط عناصر المجموعة المتقطعة. |
| [EndDate](../../aspose.cells.pivot/pivotfieldgroupoptions/enddate/) { get; set; } | يحصل أو يضبط القيمة النهائية لنطاق التجميع. |
| [EndNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/endnumber/) { get; set; } | يحصل أو يضبط القيمة النهائية لنطاق التجميع. |
| [GroupType](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptype/) { get; set; } | يحصل أو يضبط نوع التجميع لحقل المحور. فقط لتجميع حقل المحور الزمني. |
| [GroupTypes](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptypes/) { get; set; } | يحصل أو يضبط نوع التجميع لحقل المحور. |
| [Interval](../../aspose.cells.pivot/pivotfieldgroupoptions/interval/) { get; set; } | يحصل أو يضبط حجم الفاصل لكل مجموعة. |
| [IsAutoEnd](../../aspose.cells.pivot/pivotfieldgroupoptions/isautoend/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كانت القيمة النهائية تُحدد تلقائيًا. |
| [IsAutoStart](../../aspose.cells.pivot/pivotfieldgroupoptions/isautostart/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كانت القيمة الابتدائية تُحدد تلقائيًا. |
| [NewPivotField](../../aspose.cells.pivot/pivotfieldgroupoptions/newpivotfield/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب إنشاء حقول محورية جديدة بعد التجميع. |
| [StartDate](../../aspose.cells.pivot/pivotfieldgroupoptions/startdate/) { get; set; } | يحصل أو يضبط القيمة الابتدائية لنطاق التجميع. |
| [StartNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/startnumber/) { get; set; } | يحصل أو يضبط القيمة الابتدائية لنطاق التجميع. |

### أمثلة

```csharp

[C#]

// تحميل دفتر العمل النموذجي
Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
// الوصول إلى ورقة العمل الثانية وجدول المحور الخاص بها
PivotTable pt = wb.Worksheets[1].PivotTables[0];
// تجميع حقل الصف الأول (حقل تاريخ) حسب الأشهر والربع
PivotFieldGroupOptions options = new PivotFieldGroupOptions();
options.StartDate = new DateTime(2008, 1, 1);
options.EndDate = new DateTime(2008, 9, 5);
options.GroupTypes = new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Quarters };
pt.RowFields[0].Group(options);
// احسب بيانات جدول المحور واحفظ ملف الإخراج
pt.CalculateData();
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx");

[Visual Basic]

'Load the sample workbook
Dim wb As New Workbook("sampleGroupPivotFieldsInPivotTable.xlsx")
'Access the second worksheet and its pivot table
Dim pt As PivotTable = wb.Worksheets(1).PivotTables(0)
'Group the first row field (a date field) by months and quarters
Dim options As New PivotFieldGroupOptions()
options.StartDate = New DateTime(2008, 1, 1)
options.EndDate = New DateTime(2008, 9, 5)
options.GroupTypes = New PivotGroupByType() {PivotGroupByType.Months, PivotGroupByType.Quarters}
pt.RowFields(0).Group(options)
'Calculate the pivot table data and save the output file
pt.CalculateData()
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx")
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


