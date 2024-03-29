---
title: GetFontColor
second_title: Referencia de API de Aspose.Cells para .NET
description: Obtiene el color de fuente de la celda. Cuando cambia el color debe invocar el método SetFontColor para establecer el color de fuente en la celda.
type: docs
weight: 260
url: /es/net/aspose.cells.griddesktop.data/gridcell/getfontcolor/
---
## GridCell.GetFontColor method

Obtiene el color de fuente de la celda. Cuando cambia el color, debe invocar el método "SetFontColor", para establecer el color de fuente en la celda.

```csharp
public Color GetFontColor()
```

### Valor_devuelto

devolver el color de fuente de la celda.

### Ejemplos

```csharp
[C#]
GridCell cell = gridDesktop1.GetActiveWorksheet().Cells[0, 0];
Font font = new Font("Courier New", 8, FontStyle.Italic);
cell.SetFont(font);
Color color = cell.GetFontColor();
color = Color.Black;
cell.SetFontColor(color);

[Visual Basic]
Dim cell As GridCell =  gridDesktop1.GetActiveWorksheet().Cells(0, 0) 
Dim font As Font =  New Font("Courier New",8,FontStyle.Italic) 
cell.SetFont(font)
Dim color As Color =  cell.GetFontColor() 
color = Color.Black
cell.SetFontColor(color)

```

### Ver también

* class [GridCell](../../gridcell)
* espacio de nombres [Aspose.Cells.GridDesktop.Data](../../gridcell)
* asamblea [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
