---
title: "Klasse CustomCommandButton"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.CustomCommandButton Klasse. Stellt einen benutzerdefinierten Befehlsbutton in der Registerkartenleiste des GridWeb-Steuerelements dar."
type: docs
url: /de/net/aspose.cells.gridweb/customcommandbutton/
---
## CustomCommandButton class

Stellt eine benutzerdefinierte Schaltfläche im Registerkartenbereich der GridWeb‑Steuerung dar.

```csharp
public class CustomCommandButton : Control, ISerializable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CustomCommandButton](customcommandbutton/)() | Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ClientClickEvent](../../aspose.cells.gridweb/customcommandbutton/clientclickevent/) { get; set; } | Liest oder legt den Klick-Ereignishandler auf der Clientseite fest. |
| [Command](../../aspose.cells.gridweb/customcommandbutton/command/) { get; set; } | Liest oder legt den Befehlsnamen fest. |
| [CommandType](../../aspose.cells.gridweb/customcommandbutton/commandtype/) { get; set; } | Liest oder legt den Rendering-Typ des Befehls fest. Der Typ kann Befehlsbutton oder Kontextmenüeintrag sein. |
| [DiscardInput](../../aspose.cells.gridweb/customcommandbutton/discardinput/) { get; set; } | Gibt an, ob die Benutzereingabe im Client‑Browser verworfen werden soll, wenn der Benutzer diesen Button anklickt. Kann als „Rückgängig“-Aktion verwendet werden. |
| [ImageUrl](../../aspose.cells.gridweb/customcommandbutton/imageurl/) { get; set; } | Liest oder legt die Bild‑URL des Befehlsbuttons fest. Wenn sie auf null oder einen leeren String gesetzt wird, zeigt der Button nur seinen Text an. |
| [Text](../../aspose.cells.gridweb/customcommandbutton/text/) { get; set; } | Liest oder legt den Alternativtext des Befehlsbuttons fest. |
| [ToolTip](../../aspose.cells.gridweb/customcommandbutton/tooltip/) { get; set; } | Liest oder legt den Tooltip des Befehlsbuttons fest. |
| [Width](../../aspose.cells.gridweb/customcommandbutton/width/) { get; set; } | Breite des Buttons. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetObjectData](../../aspose.cells.gridweb/customcommandbutton/getobjectdata/)(SerializationInfo, StreamingContext) | Nur intern verwendet. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


