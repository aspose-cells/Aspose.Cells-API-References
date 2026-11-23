---
title: "GridDesktop.BeforeLoadFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridDesktop événement. Se produit avant que le classeur ne soit chargé depuis le fichier"
type: docs
url: /fr/net/aspose.cells.griddesktop/griddesktop/beforeloadfile/
---
## GridDesktop.BeforeLoadFile event

Se produit avant le chargement du classeur depuis le fichier.

```csharp
public event WorkbookEventHandler BeforeLoadFile;
```

### Exemples

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

### Voir aussi

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


