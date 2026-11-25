---
title: "GridDesktop.BeforeCalculate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Evento GridDesktop. Si verifica prima del calcolo della formula nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells.griddesktop/griddesktop/beforecalculate/
---
## GridDesktop.BeforeCalculate event

Si verifica prima del calcolo della formula nella cartella di lavoro.

```csharp
public event WorkbookEventHandler BeforeCalculate;
```

### Esempi

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

### Vedi anche

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


