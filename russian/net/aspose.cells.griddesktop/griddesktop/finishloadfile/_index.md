---
title: "GridDesktop.FinishLoadFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Событие GridDesktop. Происходит, когда книга загружена"
type: docs
url: /ru/net/aspose.cells.griddesktop/griddesktop/finishloadfile/
---
## GridDesktop.FinishLoadFile event

Происходит, когда рабочая книга загружена.

```csharp
public event WorkbookEventHandler FinishLoadFile;
```

### Примеры

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

### См. также

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


