---
title: "GridCell.CreateValidation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCell-Methode. Erstellt ein Validierungsobjekt für eine Zelle"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridcell/createvalidation/
---
## GridCell.CreateValidation method

Erstellt ein Validierungsobjekt für eine Zelle.

```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| validationType | GridValidationType | Validierungstyp. |
| isRequried | Boolean | Ob der Zellenwert erforderlich ist. |

### Beispiele

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.ActiveSheet;
GridValidation v = sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression, true);
	// Setzt den numerischen Validierungsausdruck.
	v.RegEx = "\\d+";
	
[Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
	Dim v As GridValidation =  sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression,True) 
	 ' Sets to number validation expression.
	v.RegEx = "\\d+"
```

### Siehe auch

* class [GridValidation](../../gridvalidation/)
* enum [GridValidationType](../../gridvalidationtype/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


