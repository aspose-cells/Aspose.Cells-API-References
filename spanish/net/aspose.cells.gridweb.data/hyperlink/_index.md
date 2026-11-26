---
title: "Clase Hyperlink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.Hyperlink."
type: docs
url: /es/net/aspose.cells.gridweb.data/hyperlink/
---
## Hyperlink class

```csharp
[Obsolete("This class is obsolete; use GridHyperlink instead")]
public class Hyperlink
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Obtiene o establece el tipo de acción del hipervínculo. Puede ser ActionTpye.UrlLink o ActionType.CellCommand. El tipo UrlLink significa que el hipervínculo es un enlace a una página web o a un correo electrónico. Por ejemplo: "http://www.aspose.com" o "mailto:admin@aspose.com". El tipo CellCommand significa que el hipervínculo disparará un evento CellCommand, y usted puede manejar este evento. |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Obtiene el rango del hipervínculo. |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Obtiene o establece el nombre del comando de celda. |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Indica si se descarta la entrada del usuario en el navegador cliente cuando el usuario hace clic en este hipervínculo CellCommand. Podría usarse como una acción de "undo". |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Obtiene o establece la URL de la imagen del hipervínculo. Si se establece a null o cadena vacía, el hipervínculo solo mostrará su texto. |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } |  |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Obtiene o establece el texto mostrado del hipervínculo. |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Obtiene o establece la información emergente del hipervínculo. |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Obtiene o establece la cadena URL. |

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


