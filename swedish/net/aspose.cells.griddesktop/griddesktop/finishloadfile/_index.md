---
title: "GridDesktop.FinishLoadFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridDesktop-händelse. Inträffar när arbetsboken har laddats"
type: docs
url: /sv/net/aspose.cells.griddesktop/griddesktop/finishloadfile/
---
## GridDesktop.FinishLoadFile event

Uppstår när arbetsboken laddas.

```csharp
public event WorkbookEventHandler FinishLoadFile;
```

### Exempel

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

### Se även

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


