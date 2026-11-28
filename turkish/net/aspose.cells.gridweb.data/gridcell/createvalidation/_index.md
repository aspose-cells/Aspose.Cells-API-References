---
title: "GridCell.CreateValidation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCell yöntemi. Bir hücre için doğrulama nesnesi oluşturur"
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridcell/createvalidation/
---
## GridCell.CreateValidation method

Bir hücre için doğrulama nesnesi oluşturur.

```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| validationType | GridValidationType | Doğrulama türü. |
| isRequried | Boolean | Hücre değerinin gerekli olup olmadığını belirtir. |

### Örnekler

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.ActiveSheet;
GridValidation v = sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression, true);
	// Sayı doğrulama ifadesine ayarlar.
	v.RegEx = "\\d+";
	
[Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
	Dim v As GridValidation =  sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression,True) 
	 ' Sets to number validation expression.
	v.RegEx = "\\d+"
```

### Ayrıca Bakınız

* class [GridValidation](../../gridvalidation/)
* enum [GridValidationType](../../gridvalidationtype/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


