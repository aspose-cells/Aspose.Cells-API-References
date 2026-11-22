---
title: "الفئة RowFilterSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.GridWeb.Data.RowFilterSettings class. وصف ملخص لـ RowFilter"
type: docs
url: /ar/net/aspose.cells.gridweb.data/rowfiltersettings/
---
## RowFilterSettings class

وصف موجز لـ RowFilter.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | سلسلة معايير الفلتر. |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | يفعل التصفية التلقائية. سيعرض HeaderRow أزرار القائمة المنسدلة للسماح للمستخدم باختيار قيمة العمود التي سيتم تصفيتها. |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | رقم الصف النهائي لنطاق الفلتر. إذا تم تعيين هذه القيمة إلى -1، يتم استخدام رقم الصف الأخير للورقة. |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | رقم صف الرأس الذي سيعرض أزرار القائمة المنسدلة للفلتر. |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | رقم صف البداية لنطاق الفلتر. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | يبني سلسلة المعايير من إعدادات الفلتر التلقائي. |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | يمسح جميع إعدادات الفلتر ويعرض جميع الصفوف. |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | يحدد فلترًا مخصصًا. |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | يفلتر الصفوف باستخدام سلسلة المعايير. |

### ملاحظات

ملاحظة: هذه الفئة الآن مهجورة. سيتم إزالة هذه الفئة بعد 6 أشهر منذ أغسطس 2014. يمكنك استخدام GridWorksheet AddAutoFilter/FilterString لإعدادات الفلتر التلقائي/الفلتر المخصص. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


