---
title: "GridDesktop.FinishCalculate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridDesktop événement. Se produit après le calcul de la formule dans le classeur"
type: docs
url: /fr/net/aspose.cells.griddesktop/griddesktop/finishcalculate/
---
## GridDesktop.FinishCalculate event

Se produit après le calcul de la formule dans le classeur.

```csharp
public event WorkbookEventHandler FinishCalculate;
```

### Exemples

```csharp
[C#]
private void gridDesktop1_FinishCalculate(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
	MessageBox.Show("finish calculate formula!");
}

[Visual Basic]
Private  Sub gridDesktop1_FinishCalculate(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
	MessageBox.Show("finish calculate formula!")
End Sub

```

### Voir aussi

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


