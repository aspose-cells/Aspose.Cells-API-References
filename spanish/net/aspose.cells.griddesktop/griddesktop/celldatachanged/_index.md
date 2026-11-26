---
title: "GridDesktop.CellDataChanged"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Evento GridDesktop. Ocurre cuando se cambia la propiedad de datos de la celda de la cuadrícula"
type: docs
url: /es/net/aspose.cells.griddesktop/griddesktop/celldatachanged/
---
## GridDesktop.CellDataChanged event

Ocurre cuando se cambia la propiedad de datos de la celda de la cuadrícula.

```csharp
public event CellEventHandler CellDataChanged;
```

### Ejemplos

```csharp
[C#]
private void gridDesktop1_CellDataChanged(object sender, Aspose.Cells.GridDesktop.Event.CellEventArgs e)
{
	MessageBox.Show("Cell Data changed!");
}

[Visual Basic]
Private  Sub gridDesktop1_CellDataChanged(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.CellEventArgs) Handles gridDesktop1.CellDataChanged
	MessageBox.Show("Cell Data changed!")
End Sub

```

### Ver también

* delegate [CellEventHandler](../../celleventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


