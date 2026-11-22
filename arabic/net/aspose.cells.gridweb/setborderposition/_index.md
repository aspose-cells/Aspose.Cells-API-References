---
title: "التعداد SetBorderPosition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.GridWeb.SetBorderPosition. يمثل موضع الحدود الذي سيتم تعيينه لنطاق الخلايا"
type: docs
url: /ar/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

يمثل موضع الحدود الذي سيتم تعيينه لنطاق الخلايا.

```csharp
public enum SetBorderPosition
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Top | `0` | الحد العلوي |
| Bottom | `1` | الحد السفلي |
| Left | `2` | الحد الأيسر |
| Right | `3` | الحد الأيمن |
| HorizontalMiddle | `4` | الحد السفلي |
| VerticalMiddle | `5` | حدود أفقية وسطية |
| Outline | `6` | حدود عمودية وسطى |
| Cross | `7` | حدود متقاطعة |
| None | `8` | بدون حدود |

### أمثلة

```csharp
[C#]
    GridWeb GridWeb1=new GridWeb();
	GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle);

[VB]
	GridWeb1.WorkSheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle)
```

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


