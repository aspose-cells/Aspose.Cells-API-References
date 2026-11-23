---
title: "Classe CellImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.CellImage. Représente un hyperlien avec une source d'image."
type: docs
url: /fr/net/aspose.cells.gridweb.data/cellimage/
---
## CellImage class

Représente un hyperlien avec la source d'image.

```csharp
public class CellImage : Hyperlink
```

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Obtient ou définit le type d'action de l'hyperlien. Il peut être ActionTpye.UrlLink ou ActionType.CellCommand. Le type UrlLink signifie que l'hyperlien pointe vers une page Web ou un courrier électronique. Par exemple : "http://www.aspose.com" ou "mailto:admin@aspose.com". Le type CellCommand signifie que l'hyperlien déclenchera un événement CellCommand, et vous pouvez gérer cet événement. (Hérité de [`Hyperlink`](../hyperlink/).) |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Obtient la plage de l'hyperlien. (Hérité de [`Hyperlink`](../hyperlink/).) |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Obtient ou définit le nom de la Cell Command. (Hérité de [`Hyperlink`](../hyperlink/).) |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Indique s'il faut ignorer l'entrée de l'utilisateur dans le navigateur client lorsque l'utilisateur clique sur cet hyperlien CellCommand. Peut être utilisé comme une action "annuler". (Hérité de [`Hyperlink`](../hyperlink/).) |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Obtient ou définit l'URL de l'image de l'hyperlien. Si elle est définie sur null ou une chaîne vide, l'hyperlien affichera uniquement son texte. (Hérité de [`Hyperlink`](../hyperlink/).) |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } | (Hérité de [`Hyperlink`](../hyperlink/).) |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Obtient ou définit le texte affiché de l'hyperlien. (Hérité de [`Hyperlink`](../hyperlink/).) |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Obtient ou définit l'infobulle de l'hyperlien. (Hérité de [`Hyperlink`](../hyperlink/).) |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Obtient ou définit la chaîne URL. (Hérité de [`Hyperlink`](../hyperlink/).) |

### Voir aussi

* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


