---
title: "WebCells.SetBorders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WebCells. تعيين حدود لنطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells.gridweb.data/webcells/setborders/
---
## WebCells.SetBorders method

يضبط الحدود لنطاق خلايا.

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | رقم الصف الأول للنطاق (بدءًا من الصفر). |
| firstColumn | Int32 | رقم العمود الأول للنطاق (بدءًا من الصفر). |
| rowNumber | Int32 | عدد الصفوف. |
| columnNumber | Int32 | عدد الأعمدة. |
| الموضع | SetBorderPosition | موضع الحد. |
| borderStyle | WebBorderStyle | نمط الحد. |

### أمثلة

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### انظر أيضًا

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


