---
title: FinishCalculate
second_title: Aspose.Cells för .NET API-referens
description: Uppstår efter att ha beräknat formeln i arbetsboken.
type: docs
weight: 540
url: /sv/net/aspose.cells.griddesktop/griddesktop/finishcalculate/
---
## GridDesktop.FinishCalculate event

Uppstår efter att ha beräknat formeln i arbetsboken.

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

* delegate [WorkbookEventHandler](../../workbookeventhandler)
* class [GridDesktop](../../griddesktop)
* namnutrymme [Aspose.Cells.GridDesktop](../../griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
