---
title: "GridDesktop.CellDataChanged"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridDesktop evento. Si verifica quando la proprietà dei dati della cella della griglia viene modificata"
type: docs
url: /it/net/aspose.cells.griddesktop/griddesktop/celldatachanged/
---
## GridDesktop.CellDataChanged event

Si verifica quando la proprietà dati della cella della griglia viene modificata.

```csharp
public event CellEventHandler CellDataChanged;
```

### Esempi

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

### Vedi anche

* delegate [CellEventHandler](../../celleventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


