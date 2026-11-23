---
title: "Classe ComboBox"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridDesktop.ComboBox. Représente un contrôle de liste déroulante de cellule"
type: docs
url: /fr/net/aspose.cells.griddesktop/combobox/
---
## ComboBox class

Représente un contrôle de liste déroulante de cellule.

```csharp
public class ComboBox : CellControl
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Height](../../aspose.cells.griddesktop/combobox/height/) { get; set; } | Obtient ou définit la hauteur du contrôle de liste. |
| [IsInputable](../../aspose.cells.griddesktop/combobox/isinputable/) { get; set; } | Indique si l'utilisateur peut saisir du texte dans la liste déroulante. Le texte saisi sera enregistré comme valeur de la cellule. La valeur par défaut est "false". |
| [Items](../../aspose.cells.griddesktop/combobox/items/) { get; } | Obtient un objet représentant la collection des éléments contenus dans cette ComboBox. |
| [SelectedIndex](../../aspose.cells.griddesktop/combobox/selectedindex/) { get; set; } | Obtient ou définit l'index spécifiant l'élément actuellement sélectionné. La définition de l'index appellera automatiquement la méthode GridDesktop.RunAllFormulas si la propriété GridDesktop.RecalculateFormulas est vraie. |
| [Text](../../aspose.cells.griddesktop/cellcontrol/text/) { get; set; } | Obtient ou définit le texte associé à ce contrôle.(Hérité de [`CellControl`](../cellcontrol/).) |
| [Values](../../aspose.cells.griddesktop/combobox/values/) { get; } | Obtient un objet représentant la collection des valeurs contenues dans cette ComboBox. |
| [Width](../../aspose.cells.griddesktop/combobox/width/) { get; set; } | Obtient ou définit la largeur du contrôle de liste. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetSelectedIndex](../../aspose.cells.griddesktop/combobox/setselectedindex/)(int) | Définit l'index sélectionné de la ComboBox. Cela ne calculera pas la formule. Pour calculer la formule, il faut appeler GridDesktop.RunAllFormulas manuellement. Cela ne calculera jamais automatiquement les formules, même si GridDesktop.RecalculateFormulas est vrai. |

### Voir aussi

* class [CellControl](../cellcontrol/)
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


