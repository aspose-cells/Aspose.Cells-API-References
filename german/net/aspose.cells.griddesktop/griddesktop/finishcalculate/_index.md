---
title: "GridDesktop.FinishCalculate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridDesktop-Ereignis. Tritt auf, nachdem eine Formel im Arbeitsbuch berechnet wurde"
type: docs
url: /de/net/aspose.cells.griddesktop/griddesktop/finishcalculate/
---
## GridDesktop.FinishCalculate event

Tritt nach der Berechnung einer Formel in der Arbeitsmappe auf.

```csharp
public event WorkbookEventHandler FinishCalculate;
```

### Beispiele

```csharp
[C#]
private void gridDesktop1_FinishCalculate(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
	MessageBox.Show("finish calculate formula!");
}

[Visual Basic]
Private  Sub gridDesktop1_FinishCalculate(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
	MessageBox.Show("finish calculate formula!")
End Sub

```

### Siehe auch

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


