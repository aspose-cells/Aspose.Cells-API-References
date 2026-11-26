---
title: "Clase CellImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.CellImage. Representa un hipervínculo con src de imagen"
type: docs
url: /es/net/aspose.cells.gridweb.data/cellimage/
---
## CellImage class

Representa un hipervínculo con origen de imagen.

```csharp
public class CellImage : Hyperlink
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Obtiene o establece el tipo de acción del hipervínculo. Puede ser ActionTpye.UrlLink o ActionType.CellCommand. El tipo UrlLink significa que el hipervínculo es un enlace a una página web o a un correo electrónico. Por ejemplo: "http://www.aspose.com" o "mailto:admin@aspose.com". El tipo CellCommand significa que el hipervínculo disparará un evento CellCommand, y usted puede manejar este evento.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Obtiene el rango del hipervínculo.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Obtiene o establece el nombre del comando de celda.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Indica si se debe descartar la entrada del usuario en el navegador cliente cuando el usuario hace clic en este hipervínculo CellCommand. Puede usarse como una acción de "deshacer".(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Obtiene o establece la URL de la imagen del hipervínculo. Si se establece a null o cadena vacía, el hipervínculo solo mostrará su texto.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } | (Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Obtiene o establece el texto mostrado del hipervínculo.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Obtiene o establece la información emergente del hipervínculo.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Obtiene o establece la cadena URL.(Inherited from [`Hyperlink`](../hyperlink/).) |

### Ver también

* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


