---
title: "GridDesktop.FinishCalculate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridDesktop olayı. Çalışma kitabında formül hesaplandıktan sonra gerçekleşir"
type: docs
url: /tr/net/aspose.cells.griddesktop/griddesktop/finishcalculate/
---
## GridDesktop.FinishCalculate event

Çalışma kitabında formül hesaplandıktan sonra oluşur.

```csharp
public event WorkbookEventHandler FinishCalculate;
```

### Örnekler

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

### Ayrıca Bakınız

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


