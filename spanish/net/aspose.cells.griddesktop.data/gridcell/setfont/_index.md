---
title: SetFont
second_title: Referencia de API de Aspose.Cells para .NET
description: Establece la fuente en la celda. Para mejorar el rendimiento implemente el método SetFont no implemente la propiedad Fuente.
type: docs
weight: 380
url: /es/net/aspose.cells.griddesktop.data/gridcell/setfont/
---
## GridCell.SetFont method

Establece la fuente en la celda. Para mejorar el rendimiento, implemente el método "SetFont", no implemente la propiedad "Fuente".

```csharp
public void SetFont(Font font)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| font | Font | fuente a configurar. |

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
