---
title: "Classe Hyperlink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.Hyperlink."
type: docs
url: /fr/net/aspose.cells.gridweb.data/hyperlink/
---
## Hyperlink class

```csharp
[Obsolete("This class is obsolete; use GridHyperlink instead")]
public class Hyperlink
```

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Obtient ou définit le type d'action du hyperlien. Il peut être ActionTpye.UrlLink ou ActionType.CellCommand. Le type UrlLink signifie que le hyperlien est un lien vers une page web ou un courrier électronique. Par exemple : "http://www.aspose.com" ou "mailto:admin@aspose.com". Le type CellCommand signifie que le hyperlien déclenchera un événement CellCommand, que vous pouvez gérer. |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Obtient la plage de l'hyperlien. |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Obtient ou définit le nom de la commande de cellule. |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Indique s'il faut ignorer l'entrée utilisateur dans le navigateur client lorsque l'utilisateur clique sur cet hyperlien CellCommand. Peut être utilisé comme une action "undo". |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Obtient ou définit l'URL de l'image du hyperlien. Si elle est définie sur null ou une chaîne vide, le hyperlien affichera uniquement son texte. |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } |  |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Obtient ou définit le texte affiché du hyperlien. |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Obtient ou définit l'infobulle du hyperlien. |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Obtient ou définit la chaîne URL. |

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


