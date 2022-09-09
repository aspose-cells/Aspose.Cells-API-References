---
title: Style
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente le style daffichage du document Excel tel que la police la couleur lalignement la bordure etc.
type: docs
weight: 980
url: /fr/net/aspose.cells.griddesktop/style/
---
## Style class

Représente le style d'affichage du document Excel, tel que la police, la couleur, l'alignement, la bordure, etc.

```csharp
public class Style
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Style](style)(GridDesktop) |  |

## Propriétés

| Nom | La description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor) { get; set; } | Obtient ou définit la couleur d'arrière-plan de la cellule, si le motif de style n'est pas défini sur solide, il prendra alors affect |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked) { get; set; } |  |
| [Color](../../aspose.cells.griddesktop/style/color) { get; set; } | Obtient ou définit la couleur d'ombrage de la cellule. lorsque le motif est aucun, il renvoie Color.Empty; lorsque le motif est BackgroundType.Solid, il renvoie ForegroundColor; les autres renvoient BackgroundColor |
| [Custom](../../aspose.cells.griddesktop/style/custom) { get; set; } |  |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor) { get; set; } | Obtient ou définit la couleur de premier plan d'un style. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment) { get; set; } | Obtient ou définit l'attribut d'alignement horizontal. |
| [Indent](../../aspose.cells.griddesktop/style/indent) { get; set; } | Représente le niveau m_IndentLevel pour la cellule ou la plage. Ne peut être qu'un entier de 0 à 15. |
| [NumberFormat](../../aspose.cells.griddesktop/style/numberformat) { get; set; } | Obtient ou définit le format d'affichage des nombres et des dates. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype) { get; set; } | identique à NumberFormat |
| [Pattern](../../aspose.cells.griddesktop/style/pattern) { get; set; } | Obtient ou définit le type de motif d'arrière-plan de la cellule. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation) { get; set; } | Représente l'angle de rotation du texte. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink) { get; set; } |  |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection) { get; set; } | Obtient ou définit l'attribut de direction du texte. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped) { get; set; } | Obtient ou définit une valeur indiquant si le texte d'une cellule est encapsulé. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment) { get; set; } | Obtient ou définit l'attribut d'alignement vertical. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone)() | Crée et renvoie une copie de cet objet.  **REMARQUE:** Si vous clonez un style nommé, le nom n'est pas cloné car le nom du style doit être unique. Par conséquent, le style cloné ne sera pas "égal" au style d'origine. |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor)(BorderType, Color) | Définit la couleur de la bordure spécifiée. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline)(BorderType, BorderLineType) | Définit le type de ligne de bordure de la bordure spécifiée. |

### Voir également

* espace de noms [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop)
* Assemblée [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->