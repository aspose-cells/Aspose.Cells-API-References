---
title: "GridCell.GetFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridCell. Obtiene la fuente de la celda. Cuando cambie la fuente, debe invocar el método SetFont para establecer la fuente en la celda."
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridcell/getfont/
---
## GridCell.GetFont method

Obtiene la fuente de la celda. Cuando cambie la fuente, debe invocar el método "SetFont", para establecer la fuente en la celda.

```csharp
public Font GetFont()
```

### Valor de retorno

devuelve una copia de la fuente de la celda.

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


