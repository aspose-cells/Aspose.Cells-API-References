---
title: "GridDesktop.FinishLoadFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridDesktop olayı. Çalışma kitabı yüklendiğinde gerçekleşir."
type: docs
url: /tr/net/aspose.cells.griddesktop/griddesktop/finishloadfile/
---
## GridDesktop.FinishLoadFile event

Çalışma kitabı yüklendiğinde oluşur.

```csharp
public event WorkbookEventHandler FinishLoadFile;
```

### Örnekler

```csharp
[C#]
private void gridDesktop1_FinishLoadFile(object sender, Aspose.Cells.GridDesktop.WorkBookEvents e)
{
	MessageBox.Show("finish load file!");
}

[Visual Basic]
Private  Sub gridDesktop1_FinishLoadFile(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.WorkBookEvents) Handles gridDesktop1.FinishLoadFile
	MessageBox.Show("finish load file!")
End Sub

```

### Ayrıca Bakınız

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


