---
title: "Klasse Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.Style class. Stellt den Anzeigestil von Excel‑Dokumenten dar, wie Schriftfarbe, Ausrichtung, Rahmen usw."
type: docs
url: /de/net/aspose.cells.griddesktop/style/
---
## Style class

Stellt den Anzeigestil eines Excel-Dokuments dar, wie Schriftart, Farbe, Ausrichtung, Rahmen usw.

```csharp
public class Style
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Style](style/)(GridDesktop) | Erstelle einen neuen Style für das Steuerelement. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor/) { get; set; } | Liest oder setzt die Hintergrundfarbe der Zelle, wenn das Stil‑Muster nicht auf solid gesetzt ist, wird es wirksam. |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob eine Zelle bearbeitet werden kann oder nicht. |
| [Color](../../aspose.cells.griddesktop/style/color/) { get; set; } | Liest oder setzt die Schattierungsfarbe der Zelle. Wenn das Muster none ist, wird Color.Empty zurückgegeben; wenn das Muster BackgroundType.Solid ist, wird ForegroundColor zurückgegeben; sonst wird BackgroundColor zurückgegeben. |
| [Custom](../../aspose.cells.griddesktop/style/custom/) { get; set; } | Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Style‑Objekts dar. Wenn das benutzerdefinierte Zahlenformat nicht gesetzt ist (z. B. das Zahlenformat ist eingebaut), wird \"\" zurückgegeben. |
| [Font](../../aspose.cells.griddesktop/style/font/) { get; set; } | Liest ein [`GridFont`](../../aspose.cells.griddesktop.data/gridfont/)‑Objekt. |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor/) { get; set; } | Liest oder setzt die Vordergrundfarbe eines Stils. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment/) { get; set; } | Liest oder setzt das Attribut für die horizontale Ausrichtung. |
| [Indent](../../aspose.cells.griddesktop/style/indent/) { get; set; } | Stellt das m_IndentLevel‑Level für die Zelle oder den Bereich dar. Kann nur ein ganzzahliger Wert von 0 bis 15 sein. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype/) { get; set; } | Liest oder setzt das Anzeigeformat von Zahlen und Daten. Die Formatierungsmuster unterscheiden sich je nach Region. |
| [Pattern](../../aspose.cells.griddesktop/style/pattern/) { get; set; } | Liest oder setzt den Hintergrundmuster-Typ der Zelle. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation/) { get; set; } | Stellt den Textdrehwinkel dar. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink/) { get; set; } | Gibt an, ob der Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen. |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection/) { get; set; } | Liest oder setzt das Attribut für die Textausrichtung. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Text innerhalb einer Zelle umgebrochen wird. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment/) { get; set; } | Liest oder setzt das Attribut für die vertikale Ausrichtung. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone/)() | Erstellt und gibt eine Kopie dieses Objekts zurück. **NOTE:** Wenn Sie einen benannten Stil klonen, wird der Name nicht geklont, weil Stilnamen eindeutig sein müssen. Daher wird der geklonte Stil nicht dem Originalstil "entsprechen". |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor/)(BorderType, Color) | Setzt die Farbe des angegebenen Rahmens. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline/)(BorderType, BorderLineType) | Setzt den Linientyp des angegebenen Rahmens. |

### Siehe auch

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


