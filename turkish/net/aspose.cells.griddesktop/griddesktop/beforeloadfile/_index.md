---
title: "GridDesktop.BeforeLoadFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridDesktop olayı. Çalışma kitabı dosyadan yüklenmeden önce gerçekleşir"
type: docs
url: /tr/net/aspose.cells.griddesktop/griddesktop/beforeloadfile/
---
## GridDesktop.BeforeLoadFile event

Çalışma kitabı dosyadan yüklenmeden önce gerçekleşir.

```csharp
public event WorkbookEventHandler BeforeLoadFile;
```

### Örnekler

```csharp
[C#]
private void gridDesktop1_BeforeLoadFile(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
	MessageBox.Show("before load file!");
}

[Visual Basic]
Private  Sub gridDesktop1_BeforeLoadFile(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
	MessageBox.Show("before load file!")
End Sub

```

### Ayrıca Bakınız

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


