---
title: "الفئة Timeline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Timelines.Timeline. وصف موجز لعرض الخط الزمني بسبب عدم دعم MS Excel 2003 للخط الزمني"
type: docs
url: /ar/net/aspose.cells.timelines/timeline/
---
## Timeline class

وصف موجز لعرض Timeline بسبب مايكروسوفت إكسل، لا يدعم Excel 2003 Timeline.

```csharp
public class Timeline
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Caption](../../aspose.cells.timelines/timeline/caption/) { get; set; } | يحصل أو يضبط التسمية التوضيحية لهذا الـ Timeline. |
| [CurrentLevel](../../aspose.cells.timelines/timeline/currentlevel/) { get; set; } | المستوى الزمني الحالي للـ Timeline. |
| [HeightPixel](../../aspose.cells.timelines/timeline/heightpixel/) { get; set; } | (**Obsolete.**) يرجع أو يضبط ارتفاع الخط الزمني المحدد، بالبكسل. |
| [LeftPixel](../../aspose.cells.timelines/timeline/leftpixel/) { get; set; } | (**Obsolete.**) يرجع أو يضبط الإزاحة الأفقية لشكل الخط الزمني من العمود الأيسر، بالبكسل. |
| [Name](../../aspose.cells.timelines/timeline/name/) { get; set; } | يرجع أو يضبط اسم الخط الزمني المحدد |
| [SelectionLevel](../../aspose.cells.timelines/timeline/selectionlevel/) { get; set; } | يحصل ويضبط المستوى الزمني الذي تم فيه الاختيار الحالي للـ Timeline. |
| [Shape](../../aspose.cells.timelines/timeline/shape/) { get; } | يرجع كائن [`TimelineShape`](../../aspose.cells.drawing/timelineshape/) المرتبط بهذا الـ Timeline. |
| [ShowHeader](../../aspose.cells.timelines/timeline/showheader/) { get; set; } | يشير إلى ما إذا كان سيتم عرض رأس هذا الخط الزمني. |
| [ShowHorizontalScrollbar](../../aspose.cells.timelines/timeline/showhorizontalscrollbar/) { get; set; } | يشير إلى ما إذا كان سيتم عرض شريط التمرير الأفقي. |
| [ShowSelectionLabel](../../aspose.cells.timelines/timeline/showselectionlabel/) { get; set; } | يشير إلى ما إذا كان سيتم عرض تسمية الاختيار. |
| [ShowTimeLevel](../../aspose.cells.timelines/timeline/showtimelevel/) { get; set; } | يشير إلى ما إذا كان سيتم عرض صندوق الاختيار المنسدل للمستوى الزمني. |
| [StartDate](../../aspose.cells.timelines/timeline/startdate/) { get; set; } | يحصل على ويضبط تاريخ البدء لموضع تمرير النطاق الزمني لهذا `Timeline`. |
| [TopPixel](../../aspose.cells.timelines/timeline/toppixel/) { get; set; } | (**Obsolete.**) إرجاع أو ضبط الإزاحة العمودية لشكل المخطط الزمني من صفه العلوي، بوحدات البكسل. |
| [WidthPixel](../../aspose.cells.timelines/timeline/widthpixel/) { get; set; } | (**Obsolete.**) إرجاع أو ضبط عرض المخطط الزمني المحدد، بوحدات البكسل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetSelectedDateTimeRange](../../aspose.cells.timelines/timeline/getselecteddatetimerange/)() | يحصل على النطاق المحدد للوقت والتاريخ. |
| [Select](../../aspose.cells.timelines/timeline/select/)(DateTime, DateTime, bool) | حدد العنصر بين التاريخ والوقت. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Timelines;
    using System;

    public class TimelineDemo
    {
        public static void TimelineExample()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // ملء ورقة العمل ببيانات عينة
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";

            // إنشاء نمط تاريخ
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = "m/d/yyyy";
            cells[0, 1].Value = "date";
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);
            // ضبط نمط التاريخ
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // إضافة PivotTable
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "date");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // تحديث بيانات PivotTable
            pivot.RefreshData();
            pivot.CalculateData();

            // إضافة مخطط زمني جديد باستخدام PivotTable كمصدر للبيانات
            sheet.Timelines.Add(pivot, 10, 5, "date");

            // الحصول على كائن Timeline
            Timeline timelineObj = sheet.Timelines[0];

            // ضبط خصائص Timeline
            timelineObj.Caption = "timeline caption test";
            timelineObj.Name = "timeline name test";
            timelineObj.LeftPixel = 100;
            timelineObj.TopPixel = 50;
            timelineObj.WidthPixel = 300;
            timelineObj.HeightPixel = 100;

            // احفظ المصنف
            book.Save("TimelineExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)


