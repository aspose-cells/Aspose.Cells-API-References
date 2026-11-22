---
title: "GridDesktop.CellDataChanged"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "حدث GridDesktop. يحدث عندما يتم تغيير خاصية بيانات خلية الشبكة"
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/celldatachanged/
---
## GridDesktop.CellDataChanged event

يحدث عندما يتم تغيير خاصية البيانات لخلية الشبكة.

```csharp
public event CellEventHandler CellDataChanged;
```

### أمثلة

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

### انظر أيضًا

* delegate [CellEventHandler](../../celleventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


