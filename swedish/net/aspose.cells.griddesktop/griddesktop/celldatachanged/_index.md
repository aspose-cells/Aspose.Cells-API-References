---
title: "GridDesktop.CellDataChanged"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridDesktop händelse. Inträffar när egenskapen för rutcellens data ändras"
type: docs
url: /sv/net/aspose.cells.griddesktop/griddesktop/celldatachanged/
---
## GridDesktop.CellDataChanged event

Uppstår när gridcellens dataegenskap ändras.

```csharp
public event CellEventHandler CellDataChanged;
```

### Exempel

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

### Se även

* delegate [CellEventHandler](../../celleventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


