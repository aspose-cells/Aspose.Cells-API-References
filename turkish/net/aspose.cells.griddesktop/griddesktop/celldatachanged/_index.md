---
title: "GridDesktop.CellDataChanged"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridDesktop olay. Grid hücre veri özelliği değiştirildiğinde oluşur"
type: docs
url: /tr/net/aspose.cells.griddesktop/griddesktop/celldatachanged/
---
## GridDesktop.CellDataChanged event

Izgara hücresi veri özelliği değiştirildiğinde oluşur.

```csharp
public event CellEventHandler CellDataChanged;
```

### Örnekler

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

### Ayrıca Bakınız

* delegate [CellEventHandler](../../celleventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


