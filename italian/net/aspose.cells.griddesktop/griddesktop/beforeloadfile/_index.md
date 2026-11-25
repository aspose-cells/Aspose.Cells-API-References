---
title: "GridDesktop.BeforeLoadFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridDesktop evento. Si verifica prima che la cartella di lavoro sia caricata dal file"
type: docs
url: /it/net/aspose.cells.griddesktop/griddesktop/beforeloadfile/
---
## GridDesktop.BeforeLoadFile event

Si verifica prima che la cartella di lavoro venga caricata dal file.

```csharp
public event WorkbookEventHandler BeforeLoadFile;
```

### Esempi

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

### Vedi anche

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


