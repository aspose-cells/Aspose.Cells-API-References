---
title: "GridCell.CreateValidation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCell method. Skapar ett valideringsobjekt för en cell"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcell/createvalidation/
---
## GridCell.CreateValidation method

Skapar ett valideringsobjekt för en cell.

```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| validationType | GridValidationType | Valideringstyp. |
| isRequried | Boolean | Om cellvärdet är obligatoriskt. |

### Exempel

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.ActiveSheet;
GridValidation v = sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression, true);
	// Ställer in nummervalideringsuttryck.
	v.RegEx = "\\d+";
	
[Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
	Dim v As GridValidation =  sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression,True) 
	 ' Sets to number validation expression.
	v.RegEx = "\\d+"
```

### Se även

* class [GridValidation](../../gridvalidation/)
* enum [GridValidationType](../../gridvalidationtype/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


