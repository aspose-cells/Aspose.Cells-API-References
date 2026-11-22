---
title: "PivotField.Top10AutoShow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تُكوّن إعدادات Top10 AutoShow لهذا الحقل المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

يضبط إعدادات Top10 AutoShow لهذا الحقل المحوري.

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isAutoShow | منطقي | true لتمكين AutoShow؛ false لتعطيله. |
| isTop | منطقي | إذا كان true، يُظهر العناصر العليا؛ إذا كان false، يُظهر العناصر السفلى. |
| عدد | Int32 | عدد العناصر العليا/السفلى التي سيتم عرضها. |
| rankBy | Int32 | فهرس حقل البيانات المستخدم للترتيب. استخدم -1 للترتيب بناءً على قيم العنصر المحوري نفسه. |

### ملاحظات

هذه الطريقة تُكوّن [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/).

تنسيق XLS الثنائي: AutoShow (Top10) هو الخيار الأصلي والوحيد المدعوم.

XLSX (OpenXML): يدعم تنسيق الملف الأساسي Top10 AutoShow، لكن واجهة المستخدم في Excel 2007 وما بعده تُظهر ذلك فقط عبر مرشح Top10. إذا لم تكن توافقية XLS مطلوبة، يُنصح باستخدام مرشح Top10 بدلاً من ذلك.

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


