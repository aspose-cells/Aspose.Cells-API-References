---
title: "GridDesktop.FinishLoadFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridDesktop evento. Si verifica quando la cartella di lavoro è caricata"
type: docs
url: /it/net/aspose.cells.griddesktop/griddesktop/finishloadfile/
---
## GridDesktop.FinishLoadFile event

Si verifica quando la cartella di lavoro viene caricata.

```csharp
public event WorkbookEventHandler FinishLoadFile;
```

### Esempi

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

### Vedi anche

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


