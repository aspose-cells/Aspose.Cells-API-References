---
title: "GridCell.Formula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GridCell. Obtiene o establece una fórmula de la celda"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

Obtiene o establece una fórmula de la celda.

```csharp
public string Formula { get; set; }
```

### Observaciones

Una cadena de fórmula siempre comienza con un signo igual (=). Y por favor, use siempre la coma (,) como delimitador de parámetros, como "=SUM(A1, E1, H2)".

El usuario puede establecer cualquier fórmula en el archivo de diseño de Workbook. Aspose.Cells mantendrá todas las fórmulas. Si el usuario usa esta propiedad para establecer una fórmula en una celda, se admite la mayor parte de las funciones integradas de Workbook. Y hay más por venir. Si tiene alguna necesidad especial para las funciones integradas de Workbook, por favor háganoslo saber.

### Ejemplos

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### Ver también

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


