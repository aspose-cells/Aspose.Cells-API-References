---
title: "GridDesktop.CellDataChanged"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridDesktop-Ereignis. Tritt auf, wenn die Daten-Eigenschaft der Gridzelle geändert wird"
type: docs
url: /de/net/aspose.cells.griddesktop/griddesktop/celldatachanged/
---
## GridDesktop.CellDataChanged event

Tritt auf, wenn die Dateneigenschaft der Gridzelle geändert wird.

```csharp
public event CellEventHandler CellDataChanged;
```

### Beispiele

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

### Siehe auch

* delegate [CellEventHandler](../../celleventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


