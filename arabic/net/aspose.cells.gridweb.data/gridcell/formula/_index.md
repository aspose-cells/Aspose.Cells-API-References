---
title: "GridCell.Formula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GridCell. تحصل أو تعين صيغة الـ GridCell"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridcell/formula/
---
## GridCell.Formula property

تحصل أو تعين صيغة الـ [`GridCell`](../).

```csharp
public string Formula { get; set; }
```

### ملاحظات

دائمًا ما يبدأ نص الصيغة بعلامة مساواة (=). ويرجى دائمًا استخدام الفاصلة (,) كفاصل للمعاملات، مثل "=SUM(A1, E1, H2)".

يمكن للمستخدم تعيين أي صيغة في ملف مصمم المصنف. سيحافظ Aspose.Cells على جميع الصيغ. إذا استخدم المستخدم هذه الخاصية لتعيين صيغة لخلية، فإن الجزء الأكبر من الدوال المدمجة في المصنف مدعوم. والمزيد قادم. إذا كان لديك أي احتياجات خاصة للدوال المدمجة في المصنف، يرجى إبلاغنا.

### أمثلة

```csharp
[C#]

ridWeb GridWeb1 = new GridWeb();
ridWorksheet sheet = GridWeb1.ActiveSheet;
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1";

Visual Basic]

im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1"
```

### انظر أيضًا

* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


