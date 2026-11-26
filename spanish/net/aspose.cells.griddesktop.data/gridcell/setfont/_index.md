---
title: "GridCell.SetFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridCell. Establece la fuente en la celda. Para mejorar el rendimiento implemente el método SetFont y no implemente la propiedad Font."
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridcell/setfont/
---
## GridCell.SetFont method

Establece la fuente en la celda. Para mejorar el rendimiento, implemente el método "SetFont", no implemente la propiedad "Font".

```csharp
public void SetFont(Font font)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fuente | Fuente | fuente a establecer. |

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

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


