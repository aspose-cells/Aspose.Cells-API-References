---
title: "GridDesktop.FinishCalculate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridDesktop event. Uppstår efter att formeln beräknats i arbetsboken"
type: docs
url: /sv/net/aspose.cells.griddesktop/griddesktop/finishcalculate/
---
## GridDesktop.FinishCalculate event

Uppstår efter att formeln beräknats i arbetsboken.

```csharp
public event WorkbookEventHandler FinishCalculate;
```

### Exempel

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

### Se även

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


