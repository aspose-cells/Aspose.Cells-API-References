---
title: "GridCell.CreateValidation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridCell. تنشئ كائن تحقق للخلية"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridcell/createvalidation/
---
## GridCell.CreateValidation method

ينشئ كائن تحقق لخلية.

```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| validationType | GridValidationType | نوع التحقق. |
| isRequried | منطقي | ما إذا كانت قيمة الخلية مطلوبة. |

### أمثلة

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.ActiveSheet;
GridValidation v = sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression, true);
	// يحدد تعبير التحقق الرقمي.
	v.RegEx = "\\d+";
	
[Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
	Dim v As GridValidation =  sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression,True) 
	 ' Sets to number validation expression.
	v.RegEx = "\\d+"
```

### انظر أيضًا

* class [GridValidation](../../gridvalidation/)
* enum [GridValidationType](../../gridvalidationtype/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


