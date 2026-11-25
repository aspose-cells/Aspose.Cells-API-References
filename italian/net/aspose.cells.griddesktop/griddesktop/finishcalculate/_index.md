---
title: "GridDesktop.FinishCalculate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Evento GridDesktop. Si verifica dopo il calcolo della formula nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells.griddesktop/griddesktop/finishcalculate/
---
## GridDesktop.FinishCalculate event

Si verifica dopo il calcolo della formula nella cartella di lavoro.

```csharp
public event WorkbookEventHandler FinishCalculate;
```

### Esempi

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

### Vedi anche

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


