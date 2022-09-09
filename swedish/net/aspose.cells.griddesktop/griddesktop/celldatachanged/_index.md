---
title: CellDataChanged
second_title: Aspose.Cells för .NET API-referens
description: Uppstår när rutnätscelldataegenskapen ändras.
type: docs
weight: 430
url: /sv/net/aspose.cells.griddesktop/griddesktop/celldatachanged/
---
## GridDesktop.CellDataChanged event

Uppstår när rutnätscelldataegenskapen ändras.

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

* delegate [CellEventHandler](../../celleventhandler)
* class [GridDesktop](../../griddesktop)
* namnutrymme [Aspose.Cells.GridDesktop](../../griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->