---
title: "GridDesktop.FinishCalculate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Evento de GridDesktop. Ocurre después de calcular la fórmula en el libro de trabajo"
type: docs
url: /es/net/aspose.cells.griddesktop/griddesktop/finishcalculate/
---
## GridDesktop.FinishCalculate event

Ocurre después de calcular la fórmula en el libro de trabajo.

```csharp
public event WorkbookEventHandler FinishCalculate;
```

### Ejemplos

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

### Ver también

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


