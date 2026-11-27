---
title: "Klass Hyperlink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.Hyperlink-klass."
type: docs
url: /sv/net/aspose.cells.gridweb.data/hyperlink/
---
## Hyperlink class

```csharp
[Obsolete("This class is obsolete; use GridHyperlink instead")]
public class Hyperlink
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Hämtar eller anger hyperlänkens åtgärdstyp. Den kan vara ActionTpye.UrlLink eller ActionType.CellCommand. UrlLink-typen betyder att hyperlänken är en länk till en webbsida eller ett e‑postmeddelande. Till exempel: "http://www.aspose.com" eller "mailto:admin@aspose.com". CellCommand-typen betyder att hyperlänken utlöser en CellCommand‑händelse, och du kan hantera denna händelse. |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Hämtar intervallet för hyperlänken. |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Hämtar eller anger Cell Command-namnet. |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Anger om användarinmatning i klientens webbläsare ska förkastas när användaren klickar på denna CellCommand‑hyperlänk. Kan användas som en "ångra"‑åtgärd. |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Hämtar eller anger hyperlänkens bild‑url. Om den sätts till null eller en tom sträng visas endast hyperlänkens text. |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } |  |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Hämtar eller anger den visade texten för hyperlänken. |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Hämtar eller anger verktygstipset för hyperlänken. |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Hämtar eller anger URL‑strängen. |

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


