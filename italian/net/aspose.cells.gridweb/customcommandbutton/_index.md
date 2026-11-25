---
title: "Classe CustomCommandButton"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.CustomCommandButton. Rappresenta un pulsante di comando personalizzato nella barra delle schede del controllo GridWeb."
type: docs
url: /it/net/aspose.cells.gridweb/customcommandbutton/
---
## CustomCommandButton class

Rappresenta un pulsante di comando personalizzato nella barra delle schede del controllo GridWeb.

```csharp
public class CustomCommandButton : Control, ISerializable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CustomCommandButton](customcommandbutton/)() | Costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ClientClickEvent](../../aspose.cells.gridweb/customcommandbutton/clientclickevent/) { get; set; } | Ottiene o imposta il gestore dell'evento click lato client. |
| [Command](../../aspose.cells.gridweb/customcommandbutton/command/) { get; set; } | Ottiene o imposta il nome del comando. |
| [CommandType](../../aspose.cells.gridweb/customcommandbutton/commandtype/) { get; set; } | Ottiene o imposta il tipo di rendering del comando. Il tipo può essere pulsante di comando o voce di menu contestuale. |
| [DiscardInput](../../aspose.cells.gridweb/customcommandbutton/discardinput/) { get; set; } | Indica se scartare l'input dell'utente nel browser client quando l'utente clicca questo pulsante. Può essere usato come azione di "annulla". |
| [ImageUrl](../../aspose.cells.gridweb/customcommandbutton/imageurl/) { get; set; } | Ottiene o imposta l'URL dell'immagine del pulsante di comando. Se impostato a null o stringa vuota, il pulsante mostrerà solo il suo testo. |
| [Text](../../aspose.cells.gridweb/customcommandbutton/text/) { get; set; } | Ottiene o imposta il testo alternativo del pulsante di comando. |
| [ToolTip](../../aspose.cells.gridweb/customcommandbutton/tooltip/) { get; set; } | Ottiene o imposta il tooltip del pulsante di comando. |
| [Width](../../aspose.cells.gridweb/customcommandbutton/width/) { get; set; } | Larghezza del pulsante. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetObjectData](../../aspose.cells.gridweb/customcommandbutton/getobjectdata/)(SerializationInfo, StreamingContext) | Utilizzato solo internamente. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


