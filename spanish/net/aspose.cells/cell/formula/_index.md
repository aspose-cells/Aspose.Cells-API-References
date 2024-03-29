---
title: Formula
second_title: Referencia de API de Aspose.Cells para .NET
description: Obtiene o establece una fórmula delCellaspose.cells/cell .
type: docs
weight: 90
url: /es/net/aspose.cells/cell/formula/
---
## Cell.Formula property

Obtiene o establece una fórmula del[`Cell`](../../cell) .

```csharp
public string Formula { get; set; }
```

### Observaciones

Una cadena de fórmula siempre comienza con un signo igual (=). Y utilice siempre la coma (,) como delimitador de parámetros, como "=SUM(A1, E1, H2)".

### Ejemplos

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;
cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1";

[Visual Basic]

Dim excel As Workbook =  New Workbook() 
Dim cells As Cells =  excel.Worksheets(0).Cells 
cells("B6").Formula = "=SUM(B2:B5, E1) + sheet1!A1"
```

### Ver también

* class [Cell](../../cell)
* espacio de nombres [Aspose.Cells](../../cell)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
