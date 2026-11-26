---
title: "GridDesktop.CellDataChanged"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Событие GridDesktop. Происходит, когда свойство данных ячейки изменяется"
type: docs
url: /ru/net/aspose.cells.griddesktop/griddesktop/celldatachanged/
---
## GridDesktop.CellDataChanged event

Происходит, когда свойство данных ячейки сетки изменяется.

```csharp
public event CellEventHandler CellDataChanged;
```

### Примеры

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

### См. также

* delegate [CellEventHandler](../../celleventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


