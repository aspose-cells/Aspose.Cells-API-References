---
title: "GridDesktop.BeforeLoadFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridDesktop-händelse. Inträffar innan arbetsboken laddas från fil"
type: docs
url: /sv/net/aspose.cells.griddesktop/griddesktop/beforeloadfile/
---
## GridDesktop.BeforeLoadFile event

Uppstår innan arbetsboken laddas från fil.

```csharp
public event WorkbookEventHandler BeforeLoadFile;
```

### Exempel

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

### Se även

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


