---
title: "GridCell.SetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridCell. Establece el estilo a la celda. Para mejorar el rendimiento, implemente el método SetStyle y no implemente la propiedad Style"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridcell/setstyle/
---
## GridCell.SetStyle method

Establece el estilo en la celda. Para mejorar el rendimiento, implemente el método "SetStyle", no implemente la propiedad "Style".

```csharp
public void SetStyle(Style value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | estilo a establecer. |

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


