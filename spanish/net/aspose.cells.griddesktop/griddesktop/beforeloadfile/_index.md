---
title: BeforeLoadFile
second_title: Referencia de API de Aspose.Cells para .NET
description: Ocurre antes de que el libro de trabajo se cargue desde el archivo.
type: docs
weight: 380
url: /es/net/aspose.cells.griddesktop/griddesktop/beforeloadfile/
---
## GridDesktop.BeforeLoadFile event

Ocurre antes de que el libro de trabajo se cargue desde el archivo.

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

* delegate [WorkbookEventHandler](../../workbookeventhandler)
* class [GridDesktop](../../griddesktop)
* espacio de nombres [Aspose.Cells.GridDesktop](../../griddesktop)
* asamblea [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
