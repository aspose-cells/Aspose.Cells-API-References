---
title: "GridDesktop.BeforeCalculate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Событие GridDesktop. Происходит перед вычислением формулы в рабочей книге"
type: docs
url: /ru/net/aspose.cells.griddesktop/griddesktop/beforecalculate/
---
## GridDesktop.BeforeCalculate event

Событие происходит перед вычислением формулы в книге.

```csharp
public event WorkbookEventHandler BeforeCalculate;
```

### Примеры

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

### См. также

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


