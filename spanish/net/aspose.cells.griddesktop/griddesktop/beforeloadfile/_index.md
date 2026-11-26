---
title: "GridDesktop.BeforeLoadFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "GridDesktop evento. Ocurre antes de que el libro de trabajo se cargue desde el archivo"
type: docs
url: /es/net/aspose.cells.griddesktop/griddesktop/beforeloadfile/
---
## GridDesktop.BeforeLoadFile event

Ocurre antes de que el libro de trabajo se cargue desde un archivo.

```csharp
public event WorkbookEventHandler BeforeLoadFile;
```

### Ejemplos

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

### Ver también

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


