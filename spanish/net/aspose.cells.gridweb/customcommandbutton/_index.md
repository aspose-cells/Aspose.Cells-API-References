---
title: "Clase CustomCommandButton"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.CustomCommandButton. Representa un botón de comando personalizado en la barra de pestañas del control GridWeb."
type: docs
url: /es/net/aspose.cells.gridweb/customcommandbutton/
---
## CustomCommandButton class

Representa un botón de comando personalizado en la barra de pestañas del control GridWeb.

```csharp
public class CustomCommandButton : Control, ISerializable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CustomCommandButton](customcommandbutton/)() | Constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ClientClickEvent](../../aspose.cells.gridweb/customcommandbutton/clientclickevent/) { get; set; } | Obtiene o establece el controlador del evento de clic en el lado del cliente. |
| [Command](../../aspose.cells.gridweb/customcommandbutton/command/) { get; set; } | Obtiene o establece el nombre del comando. |
| [CommandType](../../aspose.cells.gridweb/customcommandbutton/commandtype/) { get; set; } | Obtiene o establece el tipo de renderizado del comando. El tipo puede ser botón de comando o elemento de menú contextual. |
| [DiscardInput](../../aspose.cells.gridweb/customcommandbutton/discardinput/) { get; set; } | Indica si se debe descartar la entrada del usuario en el navegador cliente cuando el usuario hace clic en este botón. Puede usarse como una acción de "deshacer". |
| [ImageUrl](../../aspose.cells.gridweb/customcommandbutton/imageurl/) { get; set; } | Obtiene o establece la URL de la imagen del botón de comando. Si se establece a null o cadena vacía, el botón solo mostrará su texto. |
| [Text](../../aspose.cells.gridweb/customcommandbutton/text/) { get; set; } | Obtiene o establece el texto alternativo del botón de comando. |
| [ToolTip](../../aspose.cells.gridweb/customcommandbutton/tooltip/) { get; set; } | Obtiene o establece la información emergente del botón de comando. |
| [Width](../../aspose.cells.gridweb/customcommandbutton/width/) { get; set; } | Ancho del botón. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetObjectData](../../aspose.cells.gridweb/customcommandbutton/getobjectdata/)(SerializationInfo, StreamingContext) | Solo de uso interno. |

### Ejemplos

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

### Ver también

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


