---
title: "Klasse Hyperlink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.Hyperlink Klasse."
type: docs
url: /de/net/aspose.cells.gridweb.data/hyperlink/
---
## Hyperlink class

```csharp
[Obsolete("This class is obsolete; use GridHyperlink instead")]
public class Hyperlink
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Liest oder setzt den Aktionstyp des Hyperlinks. Er kann ActionTpye.UrlLink oder ActionType.CellCommand sein. Der UrlLink‑Typ bedeutet, dass der Hyperlink ein Link zu einer Webseite oder einer E‑Mail‑Empfangsadresse ist. Zum Beispiel: "http://www.aspose.com" oder "mailto:admin@aspose.com". Der CellCommand‑Typ bedeutet, dass der Hyperlink ein CellCommand‑Ereignis auslöst, das Sie behandeln können. |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Ermittelt den Bereich des Hyperlinks. |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Liest oder setzt den Namen des Cell Command. |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Gibt an, ob Benutzereingaben im Client-Browser verworfen werden sollen, wenn der Benutzer diesen CellCommand-Hyperlink anklickt. Kann als "Rückgängig"-Aktion verwendet werden. |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Liest oder setzt die Bild‑URL des Hyperlinks. Wenn sie auf null oder einen leeren String gesetzt wird, zeigt der Hyperlink nur seinen Text an. |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } |  |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Liest oder setzt den angezeigten Text des Hyperlinks. |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Liest oder setzt den Tooltip des Hyperlinks. |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Ermittelt oder legt die URL-Zeichenkette fest. |

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


