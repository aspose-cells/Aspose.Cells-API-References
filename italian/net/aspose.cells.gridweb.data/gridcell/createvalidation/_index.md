---
title: "GridCell.CreateValidation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridCell. Crea un oggetto di convalida per una cella"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridcell/createvalidation/
---
## GridCell.CreateValidation method

Crea un oggetto di convalida per una cella.

```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| validationType | GridValidationType | Tipo di convalida. |
| isRequried | Booleano | Indica se il valore della cella è obbligatorio. |

### Esempi

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.ActiveSheet;
GridValidation v = sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression, true);
	// Imposta l'espressione di convalida numerica.
	v.RegEx = "\\d+";
	
[Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
	Dim v As GridValidation =  sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression,True) 
	 ' Sets to number validation expression.
	v.RegEx = "\\d+"
```

### Vedi anche

* class [GridValidation](../../gridvalidation/)
* enum [GridValidationType](../../gridvalidationtype/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


