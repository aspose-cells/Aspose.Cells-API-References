---
title: "GridCell.Formula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GridCell. تحصل على صيغة الخلية أو تعيينها"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

يحصل أو يضبط صيغة الخلية.

```csharp
public string Formula { get; set; }
```

### ملاحظات

دائمًا ما يبدأ نص الصيغة بعلامة مساواة (=). ويرجى دائمًا استخدام الفاصلة (,) كفاصل للمعاملات، مثل "=SUM(A1, E1, H2)".

يمكن للمستخدم تعيين أي صيغة في ملف مصمم المصنف. سيحافظ Aspose.Cells على جميع الصيغ. إذا استخدم المستخدم هذه الخاصية لتعيين صيغة لخلية، فإن الجزء الأكبر من الدوال المدمجة في المصنف مدعوم. والمزيد قادم. إذا كان لديك أي احتياجات خاصة للدوال المدمجة في المصنف، يرجى إبلاغنا.

### أمثلة

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### انظر أيضًا

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


