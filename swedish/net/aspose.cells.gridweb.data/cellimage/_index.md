---
title: "Klass CellImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.CellImage-klass. Representerar en hyperlänk med bild‑src"
type: docs
url: /sv/net/aspose.cells.gridweb.data/cellimage/
---
## CellImage class

Representerar en hyperlänk med bildkälla.

```csharp
public class CellImage : Hyperlink
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Hämtar eller anger hyperlänkens åtgärdstyp. Den kan vara ActionTpye.UrlLink eller ActionType.CellCommand. UrlLink‑typen betyder att hyperlänken är en länk till en webbsida eller ett e‑postmeddelande. Till exempel: "http://www.aspose.com" eller "mailto:admin@aspose.com". CellCommand‑typen betyder att hyperlänken utlöser ett CellCommand‑händelse, och du kan hantera denna händelse.(ärvd från [`Hyperlink`](../hyperlink/).) |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Hämtar hyperlänkens område.(ärvd från [`Hyperlink`](../hyperlink/).) |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Hämtar eller anger Cell Command‑namnet.(ärvd från [`Hyperlink`](../hyperlink/).) |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Anger om användarinmatning i klientens webbläsare ska förkastas när användaren klickar på denna CellCommand‑hyperlänk. Kan användas som en "undo"‑åtgärd.(ärvd från [`Hyperlink`](../hyperlink/).) |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Hämtar eller anger hyperlänkens bild‑url. Om den sätts till null eller en tom sträng kommer hyperlänken endast att visa sin text.(ärvd från [`Hyperlink`](../hyperlink/).) |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } | (ärvd från [`Hyperlink`](../hyperlink/).) |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Hämtar eller anger den visade texten för hyperlänken.(ärvd från [`Hyperlink`](../hyperlink/).) |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Hämtar eller anger verktygstipset för hyperlänken.(ärvd från [`Hyperlink`](../hyperlink/).) |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Hämtar eller anger URL‑strängen.(ärvd från [`Hyperlink`](../hyperlink/).) |

### Se även

* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


