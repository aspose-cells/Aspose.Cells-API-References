---
title: "Klasse CellImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.CellImage Klasse. Stellt einen Hyperlink mit Bild‑src dar"
type: docs
url: /de/net/aspose.cells.gridweb.data/cellimage/
---
## CellImage class

Stellt einen Hyperlink mit Bild‑src dar.

```csharp
public class CellImage : Hyperlink
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Liest oder setzt den Aktionstyp des Hyperlinks. Er kann ActionTpye.UrlLink oder ActionType.CellCommand sein. Der UrlLink‑Typ bedeutet, dass der Hyperlink ein Link zu einer Webseite oder einer E‑Mail ist. Zum Beispiel: \"http://www.aspose.com\" oder \"mailto:admin@aspose.com\". Der CellCommand‑Typ bedeutet, dass der Hyperlink ein CellCommand‑Ereignis auslöst, das Sie behandeln können. (Vererbt von [`Hyperlink`](../hyperlink/).) |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Liefert den Bereich des Hyperlinks. (Vererbt von [`Hyperlink`](../hyperlink/).) |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Liest oder setzt den Namen des Cell‑Command. (Vererbt von [`Hyperlink`](../hyperlink/).) |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Gibt an, ob Benutzereingaben im Client‑Browser verworfen werden sollen, wenn der Benutzer diesen CellCommand‑Hyperlink anklickt. Kann als \"undo\"-Aktion verwendet werden. (Vererbt von [`Hyperlink`](../hyperlink/).) |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Liest oder setzt die Bild‑URL des Hyperlinks. Wenn sie auf null oder einen leeren String gesetzt wird, zeigt der Hyperlink nur seinen Text an. (Vererbt von [`Hyperlink`](../hyperlink/).) |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } | (Vererbt von [`Hyperlink`](../hyperlink/).) |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Liest oder setzt den angezeigten Text des Hyperlinks. (Vererbt von [`Hyperlink`](../hyperlink/).) |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Liest oder setzt den Tooltip des Hyperlinks. (Vererbt von [`Hyperlink`](../hyperlink/).) |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Liest oder setzt die URL‑Zeichenkette. (Vererbt von [`Hyperlink`](../hyperlink/).) |

### Siehe auch

* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


