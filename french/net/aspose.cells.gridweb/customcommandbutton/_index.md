---
title: "Classe CustomCommandButton"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridWeb.CustomCommandButton classe. Représente un bouton de commande personnalisé dans la barre d'onglets du contrôle GridWeb"
type: docs
url: /fr/net/aspose.cells.gridweb/customcommandbutton/
---
## CustomCommandButton class

Représente un bouton de commande personnalisé dans la barre d'onglets du contrôle GridWeb.

```csharp
public class CustomCommandButton : Control, ISerializable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CustomCommandButton](customcommandbutton/)() | Constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ClientClickEvent](../../aspose.cells.gridweb/customcommandbutton/clientclickevent/) { get; set; } | Obtient ou définit le gestionnaire d'événement de clic côté client. |
| [Command](../../aspose.cells.gridweb/customcommandbutton/command/) { get; set; } | Obtient ou définit le nom de la commande. |
| [CommandType](../../aspose.cells.gridweb/customcommandbutton/commandtype/) { get; set; } | Obtient ou définit le type de rendu de la commande. Le type peut être bouton de commande ou élément de menu contextuel. |
| [DiscardInput](../../aspose.cells.gridweb/customcommandbutton/discardinput/) { get; set; } | Indique si l'entrée utilisateur doit être ignorée dans le navigateur client lorsque l'utilisateur clique sur ce bouton. Peut être utilisé comme une action « annuler ». |
| [ImageUrl](../../aspose.cells.gridweb/customcommandbutton/imageurl/) { get; set; } | Obtient ou définit l'URL de l'image du bouton de commande. Si définie à null ou chaîne vide, le bouton affichera uniquement son texte. |
| [Text](../../aspose.cells.gridweb/customcommandbutton/text/) { get; set; } | Obtient ou définit le texte alternatif du bouton de commande. |
| [ToolTip](../../aspose.cells.gridweb/customcommandbutton/tooltip/) { get; set; } | Obtient ou définit l'infobulle du bouton de commande. |
| [Width](../../aspose.cells.gridweb/customcommandbutton/width/) { get; set; } | Largeur du bouton. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetObjectData](../../aspose.cells.gridweb/customcommandbutton/getobjectdata/)(SerializationInfo, StreamingContext) | Utilisé uniquement en interne. |

### Exemples

```csharp
[C#]
GridWebBean GridWeb1=ExtPage.getInstance().getBean();
CustomCommandButton button = new CustomCommandButton();
button.Command = "MyCommand";
button.ImageUrl = "images/button1.gif";
GridWeb1.CustomCommandButtons.Add(button);
[VB]
Dim button As CustomCommandButton =  New CustomCommandButton()
button.Command = "MyCommand"
button.ImageUrl = "images/button1.gif"
GridWeb1.CustomCommandButtons.Add(button)
```

### Voir aussi

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


