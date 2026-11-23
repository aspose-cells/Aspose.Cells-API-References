---
title: "GridDesktop.CellDataChanged"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridDesktop événement. Se produit lorsque la propriété de données de la cellule de la grille est modifiée"
type: docs
url: /fr/net/aspose.cells.griddesktop/griddesktop/celldatachanged/
---
## GridDesktop.CellDataChanged event

Se produit lorsque la propriété de données de la cellule de la grille est modifiée.

```csharp
public event CellEventHandler CellDataChanged;
```

### Exemples

```csharp
[C#]
private void gridDesktop1_CellDataChanged(object sender, Aspose.Cells.GridDesktop.Event.CellEventArgs e)
{
	MessageBox.Show("Cell Data changed!");
}

[Visual Basic]
Private  Sub gridDesktop1_CellDataChanged(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.CellEventArgs) Handles gridDesktop1.CellDataChanged
	MessageBox.Show("Cell Data changed!")
End Sub

```

### Voir aussi

* delegate [CellEventHandler](../../celleventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


