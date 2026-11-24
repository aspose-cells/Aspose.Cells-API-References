---
title: "GridDesktop.BeforeCalculate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridDesktop Ereignis. Tritt auf, bevor Formeln im Arbeitsbuch berechnet werden."
type: docs
url: /de/net/aspose.cells.griddesktop/griddesktop/beforecalculate/
---
## GridDesktop.BeforeCalculate event

Tritt auf, bevor die Formel in der Arbeitsmappe berechnet wird.

```csharp
public event WorkbookEventHandler BeforeCalculate;
```

### Beispiele

```csharp
[C#]
private void gridDesktop1_BeforeCalculate(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
	MessageBox.Show("before calculate formula!");
}

[Visual Basic]
Private  Sub gridDesktop1_BeforeCalculate(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
	MessageBox.Show("before calculate formula!")
End Sub

```

### Siehe auch

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


