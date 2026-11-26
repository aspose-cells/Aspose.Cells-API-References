---
title: "GridCell.Formula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GridCell. Obtiene o establece una fórmula del GridCell"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridcell/formula/
---
## GridCell.Formula property

Obtiene o establece una fórmula del [`GridCell`](../).

```csharp
public string Formula { get; set; }
```

### Observaciones

Una cadena de fórmula siempre comienza con un signo igual (=). Y por favor, use siempre la coma (,) como delimitador de parámetros, como "=SUM(A1, E1, H2)".

El usuario puede establecer cualquier fórmula en el archivo de diseño de Workbook. Aspose.Cells mantendrá todas las fórmulas. Si el usuario usa esta propiedad para establecer una fórmula en una celda, se admite la mayor parte de las funciones integradas de Workbook. Y hay más por venir. Si tiene alguna necesidad especial para las funciones integradas de Workbook, por favor háganoslo saber.

### Ejemplos

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

### Ver también

* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


