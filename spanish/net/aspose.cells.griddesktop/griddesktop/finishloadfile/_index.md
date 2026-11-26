---
title: "GridDesktop.FinishLoadFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Evento de GridDesktop. Ocurre cuando se carga el libro de trabajo"
type: docs
url: /es/net/aspose.cells.griddesktop/griddesktop/finishloadfile/
---
## GridDesktop.FinishLoadFile event

Ocurre cuando se carga el libro de trabajo.

```csharp
public event WorkbookEventHandler FinishLoadFile;
```

### Ejemplos

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

### Ver también

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


