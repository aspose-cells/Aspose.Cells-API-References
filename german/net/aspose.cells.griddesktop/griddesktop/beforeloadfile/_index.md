---
title: "GridDesktop.BeforeLoadFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridDesktop-Ereignis. Tritt auf, bevor die Arbeitsmappe aus einer Datei geladen wird"
type: docs
url: /de/net/aspose.cells.griddesktop/griddesktop/beforeloadfile/
---
## GridDesktop.BeforeLoadFile event

Tritt auf, bevor die Arbeitsmappe aus einer Datei geladen wird.

```csharp
public event WorkbookEventHandler BeforeLoadFile;
```

### Beispiele

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

### Siehe auch

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


