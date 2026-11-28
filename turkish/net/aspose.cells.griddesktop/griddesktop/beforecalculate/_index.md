---
title: "GridDesktop.BeforeCalculate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridDesktop event. Çalışma kitabında formül hesaplamadan önce gerçekleşir"
type: docs
url: /tr/net/aspose.cells.griddesktop/griddesktop/beforecalculate/
---
## GridDesktop.BeforeCalculate event

Çalışma kitabında formül hesaplanmadan önce gerçekleşir.

```csharp
public event WorkbookEventHandler BeforeCalculate;
```

### Örnekler

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

### Ayrıca Bakınız

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


