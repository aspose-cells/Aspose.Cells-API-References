---
title: "Klass CustomCommandButton"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.CustomCommandButton-klass. Representerar en anpassad kommandoknapp i flikfältet för GridWeb-kontrollen"
type: docs
url: /sv/net/aspose.cells.gridweb/customcommandbutton/
---
## CustomCommandButton class

Representerar en anpassad kommandoknapp i flikfältet för GridWeb‑kontrollen.

```csharp
public class CustomCommandButton : Control, ISerializable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CustomCommandButton](customcommandbutton/)() | Standardkonstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ClientClickEvent](../../aspose.cells.gridweb/customcommandbutton/clientclickevent/) { get; set; } | Hämtar eller anger klickhändelsehanteraren på klientsidan. |
| [Command](../../aspose.cells.gridweb/customcommandbutton/command/) { get; set; } | Hämtar eller anger kommandonamnet. |
| [CommandType](../../aspose.cells.gridweb/customcommandbutton/commandtype/) { get; set; } | Hämtar eller anger renderings‑typen för kommandot. Typen kan vara kommandoknapp eller kontextmenyalternativ. |
| [DiscardInput](../../aspose.cells.gridweb/customcommandbutton/discardinput/) { get; set; } | Indikerar om användarinmatning ska förkastas i klientens webbläsare när användaren klickar på den här knappen. Kan användas som en "undo"‑åtgärd. |
| [ImageUrl](../../aspose.cells.gridweb/customcommandbutton/imageurl/) { get; set; } | Hämtar eller anger kommandoknappens bild‑URL. Om den sätts till null eller tom sträng visas endast knappens text. |
| [Text](../../aspose.cells.gridweb/customcommandbutton/text/) { get; set; } | Hämtar eller anger alternativ text för kommandoknappen. |
| [ToolTip](../../aspose.cells.gridweb/customcommandbutton/tooltip/) { get; set; } | Hämtar eller anger verktygstipset för kommandoknappen. |
| [Width](../../aspose.cells.gridweb/customcommandbutton/width/) { get; set; } | Knappens bredd. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetObjectData](../../aspose.cells.gridweb/customcommandbutton/getobjectdata/)(SerializationInfo, StreamingContext) | Endast för internt bruk. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


