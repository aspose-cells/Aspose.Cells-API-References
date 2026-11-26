---
title: "GridCell.CreateValidation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridCell. Crea un objeto de validación para una celda"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridcell/createvalidation/
---
## GridCell.CreateValidation method

Crea un objeto de validación para una celda.

```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| validationType | GridValidationType | Tipo de validación. |
| isRequried | Booleano | Indica si el valor de la celda es obligatorio. |

### Ejemplos

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.ActiveSheet;
GridValidation v = sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression, true);
	// Establece la expresión de validación numérica.
	v.RegEx = "\\d+";
	
[Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
	Dim v As GridValidation =  sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression,True) 
	 ' Sets to number validation expression.
	v.RegEx = "\\d+"
```

### Ver también

* class [GridValidation](../../gridvalidation/)
* enum [GridValidationType](../../gridvalidationtype/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


