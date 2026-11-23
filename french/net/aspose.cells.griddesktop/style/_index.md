---
title: "Classe Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridDesktop.Style. Représente le style d'affichage des documents Excel tels que la couleur de police, l'alignement, la bordure, etc."
type: docs
url: /fr/net/aspose.cells.griddesktop/style/
---
## Style class

Représente le style d'affichage d'un document Excel, tel que la police, la couleur, l'alignement, la bordure, etc.

```csharp
public class Style
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Style](style/)(GridDesktop) | créez un nouveau Style pour le contrôle |

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor/) { get; set; } | Obtient ou définit la couleur d'arrière-plan de la cellule, si le motif du style n'est pas réglé sur solide, alors il prendra effet |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked/) { get; set; } | Obtient ou définit une valeur indiquant si une cellule peut être modifiée ou non. |
| [Color](../../aspose.cells.griddesktop/style/color/) { get; set; } | Obtient ou définit la couleur d'ombrage de la cellule. lorsque le motif est none, il renvoie Color.Empty ; lorsque le motif est BackgroundType.Solid, il renvoie ForegroundColor ; dans les autres cas il renvoie BackgroundColor |
| [Custom](../../aspose.cells.griddesktop/style/custom/) { get; set; } | Représente la chaîne de format numérique personnalisé de cet objet style. Si le format numérique personnalisé n'est pas défini (par exemple, le format numérique est intégré), "" sera retourné. |
| [Font](../../aspose.cells.griddesktop/style/font/) { get; set; } | Obtient un objet [`GridFont`](../../aspose.cells.griddesktop.data/gridfont/). |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor/) { get; set; } | Obtient ou définit la couleur de premier plan d'un style. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment/) { get; set; } | Obtient ou définit l'attribut d'alignement horizontal. |
| [Indent](../../aspose.cells.griddesktop/style/indent/) { get; set; } | Représente le niveau m_IndentLevel pour la cellule ou la plage. Ne peut être qu'un entier de 0 à 15. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype/) { get; set; } | Obtient ou définit le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions. |
| [Pattern](../../aspose.cells.griddesktop/style/pattern/) { get; set; } | Obtient ou définit le type de motif d'arrière-plan de la cellule. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation/) { get; set; } | Représente l'angle de rotation du texte. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink/) { get; set; } | Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible. |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection/) { get; set; } | Obtient ou définit l'attribut de direction du texte. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped/) { get; set; } | Obtient ou définit une valeur indiquant si le texte à l'intérieur d'une cellule est renvoyé à la ligne. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment/) { get; set; } | Obtient ou définit l'attribut d'alignement vertical. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone/)() | Crée et renvoie une copie de cet objet. **NOTE:** Si vous clonez un style nommé, le nom n'est pas cloné car le nom du style doit être unique. Par conséquent, le style cloné ne sera pas \"égal à\" le style original. |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor/)(BorderType, Color) | Définit la couleur de la bordure spécifiée. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline/)(BorderType, BorderLineType) | Définit le type de ligne de la bordure spécifiée. |

### Voir aussi

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


