---
title: "GridCell.GetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridCell. Obtiene el estilo de la celda. Cuando cambie el estilo, debe invocar el método SetStyle para establecer el estilo en la celda."
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridcell/getstyle/
---
## GridCell.GetStyle method

Obtiene el estilo de la celda. Cuando cambie el estilo, debe invocar el método "SetStyle", para establecer el estilo en la celda.

```csharp
public Style GetStyle()
```

### Valor de retorno

devuelve una copia del estilo de la celda.

### Ejemplos

```csharp
[C#]
Style style = sheet.GetCell(0, 0).GetStyle();
style.CellLocked = true;
style.VAlignment = VerticalAlignmentType.Top;
...
sheet.GetCell(0, 0).SetStyle(style);

[Visual Basic]
Dim style As Style =  sheet.GetCell(0,0).GetStyle() 
style.CellLocked = True
style.VAlignment = VerticalAlignmentType.Top
...
sheet.GetCell(0, 0).SetStyle(style)

```

### Ver también

* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


