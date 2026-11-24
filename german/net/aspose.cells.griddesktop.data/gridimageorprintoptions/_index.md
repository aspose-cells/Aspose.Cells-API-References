---
title: "Klasse GridImageOrPrintOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.Data.GridImageOrPrintOptions Klasse. Ermöglicht das Festlegen von Optionen beim Rendern von Arbeitsblättern zu Bildern, beim Drucken von Arbeitsblättern oder beim Rendern von Diagrammen zu Bildern."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridimageorprintoptions/
---
## GridImageOrPrintOptions class

Ermöglicht das Festlegen von Optionen beim Rendern von Arbeitsblättern zu Bildern, beim Drucken von Arbeitsblättern oder beim Rendern von Diagrammen zu Bildern.

```csharp
public class GridImageOrPrintOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridImageOrPrintOptions](gridimageorprintoptions/)() | Der Aufbau von GridImageOrPrintOptions |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße der pagesetup wird ungültig sein, und die anderen Einstellungen der pagesetup bleiben wirksam. |
| [CheckWorkbookDefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Wenn Zeichen in der Excel-Datei Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie als Block in PDF oder Bild erscheinen. Setzen Sie diesen Wert auf true, um zunächst zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen. |
| [DefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/defaultfont/) { get; set; } | Wenn Zeichen in der Excel-Datei Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie als Block in PDF oder Bild erscheinen. Setzen Sie die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode‑Zeichen darzustellen. |
| [EmbededImageNameInSvg](../../aspose.cells.griddesktop.data/gridimageorprintoptions/embededimagenameinsvg/) { get; set; } | Geben Sie den Dateinamen des eingebetteten Bildes in SVG an. Dies sollte ein voller Pfad mit Verzeichnis sein, z. B. "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/emftype/) { get; set; } | Ruft einen EmfType ab oder legt ihn fest, der das Format der Metafile angibt. Der Standardwert ist EmfPlusDual. |
| [GridlineType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/gridlinetype/) { get; set; } | Liest oder legt den Typ der Gitternetzlinien fest. |
| [HorizontalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/horizontalresolution/) { get; set; } | Liest oder setzt die horizontale Auflösung für erzeugte Bilder, in Punkten pro Zoll. Gilt für die Bildgenerierungsmethode, außer bei Emf-Formatbildern. |
| [ImageType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/imagetype/) { get; set; } | Liest oder setzt das Format der erzeugten Bilder. Standardwert: PNG. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Gibt an, ob die Schriftart eines Zeichens nur dann ersetzt werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist. |
| [IsOptimized](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isoptimized/) { get; set; } | Gibt an, ob die Ausgabeelemente optimiert werden sollen. |
| [OnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onepagepersheet/) { get; set; } | Ist OnePagePerSheet true, wird der gesamte Inhalt eines Blatts im Ergebnis nur auf einer Seite ausgegeben. Die Papiergröße der Seiten­einstellungen wird ungültig, während die anderen Einstellungen der Seiten­einstellungen weiterhin wirksam bleiben. |
| [OnlyArea](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onlyarea/) { get; set; } | Wenn diese Eigenschaft true ist, wird ein Area ausgegeben und keine Skalierung wirkt. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [PageCount](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pagecount/) { get; set; } | Liest oder legt die Anzahl der zu speichernden Seiten fest. |
| [PageIndex](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pageindex/) { get; set; } | Liest oder legt den nullbasierten Index der ersten zu speichernden Seite fest. |
| [PixelFormat](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pixelformat/) { get; set; } | Ruft das Pixelformat für die erzeugten Bilder ab oder legt es fest. |
| [PrintingPage](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printingpage/) { get; set; } | Gibt an, welche Seiten nicht gedruckt werden. |
| [PrintWithStatusDialog](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printwithstatusdialog/) { get; set; } | Wenn PrintWithStatusDialog = true ist, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. Andernfalls wird kein solcher Dialog angezeigt. |
| [Quality](../../aspose.cells.griddesktop.data/gridimageorprintoptions/quality/) { get; set; } | Ruft den Wert ab oder legt ihn fest, der die Qualität der erzeugten Bilder bestimmt und nur beim Speichern von Seiten im `Jpeg`‑Format angewendet wird. Der Standardwert ist 100 |
| [SmoothingMode](../../aspose.cells.griddesktop.data/gridimageorprintoptions/smoothingmode/) { get; set; } | Gibt an, ob Glättung (Antialiasing) auf Linien, Kurven und die Kanten gefüllter Bereiche angewendet wird. Der Standardwert ist SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.griddesktop.data/gridimageorprintoptions/svgfittoviewport/) { get; set; } | Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG an den Viewport an. |
| [TextCrossType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textcrosstype/) { get; set; } | Liest oder legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [TextRenderingHint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textrenderinghint/) { get; set; } | Gibt die Qualität der Textdarstellung an. Der Standardwert ist TextRenderingHint.SystemDefault |
| [Transparent](../../aspose.cells.griddesktop.data/gridimageorprintoptions/transparent/) { get; set; } | Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll. |
| [VerticalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/verticalresolution/) { get; set; } | Liest oder setzt die vertikale Auflösung für erzeugte Bilder, in Punkten pro Zoll. Gilt für die Bildgenerierungsmethode, außer bei Emf-Formatbildern. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setdesiredsize/)(int, int) | Legt die gewünschte Breite und Höhe des Bildes fest. |
| [setRenderSheetSet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setrendersheetset/)(int[]) | Setzt die zu rendernden Arbeitsblätter. Standard ist jedes sichtbare Arbeitsblatt in der Arbeitsmappe. Nullbasierte Blattindizes. |

### Siehe auch

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


