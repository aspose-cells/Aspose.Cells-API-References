---
title: "SvgImageOptions Klasse"
linktitle: "SvgImageOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SvgImageOptions Klasse. Kapselt das Objekt, das svgimageoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/svgimageoptions/
---

## SvgImageOptions class

Optionen zum Erzeugen eines SVG-Bildes.

```go

type SvgImageOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewSvgImageOptions](./newsvgimageoptions/) | Konstruktor. |
| [NewSvgImageOptions_ImageOrPrintOptions](./newsvgimageoptions_imageorprintoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetImageType](./getimagetype/) | Liest oder setzt das Format der erzeugten Bilder. Standardwert: PNG. |
| [SetImageType](./setimagetype/) | Liest oder setzt das Format der erzeugten Bilder. Standardwert: PNG. |
| [GetFitToViewPort](./getfittoviewport/) | Wenn diese Eigenschaft true ist, passt das erzeugte SVG in den Viewport. |
| [SetFitToViewPort](./setfittoviewport/) | Wenn diese Eigenschaft true ist, passt das erzeugte SVG in den Viewport. |
| [GetCssPrefix](./getcssprefix/) | Liest und setzt das Präfix des CSS-Namens im SVG, der Standardwert ist eine leere Zeichenkette. |
| [SetCssPrefix](./setcssprefix/) | Liest und setzt das Präfix des CSS-Namens im SVG, der Standardwert ist eine leere Zeichenkette. |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Liest oder setzt den Typ der Schrift, die in SVG eingebettet ist. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Liest oder setzt den Typ der Schrift, die in SVG eingebettet ist. |
| [SetPrintWithStatusDialog](./setprintwithstatusdialog/) | Wenn PrintWithStatusDialog = true ist, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. Andernfalls wird kein solcher Dialog angezeigt. |
| [GetPrintWithStatusDialog](./getprintwithstatusdialog/) | Wenn PrintWithStatusDialog = true ist, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. Andernfalls wird kein solcher Dialog angezeigt. |
| [GetHorizontalResolution](./gethorizontalresolution/) | Liest oder setzt die horizontale Auflösung für erzeugte Bilder, in DPI. |
| [SetHorizontalResolution](./sethorizontalresolution/) | Liest oder setzt die horizontale Auflösung für erzeugte Bilder, in DPI. |
| [GetVerticalResolution](./getverticalresolution/) | Liest oder setzt die vertikale Auflösung für erzeugte Bilder, in DPI. |
| [SetVerticalResolution](./setverticalresolution/) | Liest oder setzt die vertikale Auflösung für erzeugte Bilder, in DPI. |
| [GetTiffCompression](./gettiffcompression/) | Liest oder setzt den Kompressionstyp, der nur beim Speichern von Seiten im <c>Tiff</c>-Format angewendet wird. |
| [SetTiffCompression](./settiffcompression/) | Liest oder setzt den Kompressionstyp, der nur beim Speichern von Seiten im <c>Tiff</c>-Format angewendet wird. |
| [GetTiffColorDepth](./gettiffcolordepth/) | Liest oder setzt die Bit-Tiefe, die nur beim Speichern von Seiten im <c>Tiff</c>-Format angewendet wird. |
| [SetTiffColorDepth](./settiffcolordepth/) | Liest oder setzt die Bit-Tiefe, die nur beim Speichern von Seiten im <c>Tiff</c>-Format angewendet wird. |
| [GetTiffBinarizationMethod](./gettiffbinarizationmethod/) | Liest oder setzt die Methode, die beim Konvertieren von Bildern in das 1‑bpp-Format verwendet wird, wenn ImageType Tiff ist und TiffCompression gleich Ccitt3 oder Ccitt4 ist. |
| [SetTiffBinarizationMethod](./settiffbinarizationmethod/) | Liest oder setzt die Methode, die beim Konvertieren von Bildern in das 1‑bpp-Format verwendet wird, wenn ImageType Tiff ist und TiffCompression gleich Ccitt3 oder Ccitt4 ist. |
| [GetPrintingPage](./getprintingpage/) | Gibt an, welche Seiten nicht gedruckt werden. |
| [SetPrintingPage](./setprintingpage/) | Gibt an, welche Seiten nicht gedruckt werden. |
| [GetQuality](./getquality/) | Liest oder setzt einen Wert, der die Qualität der erzeugten Bilder bestimmt, der nur beim Speichern von Seiten im <c>Jpeg</c>-Format angewendet wird. Der Standardwert ist 100. |
| [SetQuality](./setquality/) | Liest oder setzt einen Wert, der die Qualität der erzeugten Bilder bestimmt, der nur beim Speichern von Seiten im <c>Jpeg</c>-Format angewendet wird. Der Standardwert ist 100. |
| [GetOnePagePerSheet](./getonepagepersheet/) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blattes nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße der Seiten-einstellung wird ungültig sein, während die anderen Einstellungen der Seiten-einstellung weiterhin wirksam bleiben. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blattes nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße der Seiten-einstellung wird ungültig sein, während die anderen Einstellungen der Seiten-einstellung weiterhin wirksam bleiben. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße von PageSetup wird ungültig, während die anderen Einstellungen von PageSetup weiterhin wirksam sind. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße von PageSetup wird ungültig, während die anderen Einstellungen von PageSetup weiterhin wirksam sind. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten. |
| [GetOnlyArea](./getonlyarea/) | Wenn diese Eigenschaft true ist, wird ein Bereich ausgegeben, und keine Skalierung wird wirksam. |
| [SetOnlyArea](./setonlyarea/) | Wenn diese Eigenschaft true ist, wird ein Bereich ausgegeben, und keine Skalierung wird wirksam. |
| [GetTransparent](./gettransparent/) | Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll. |
| [SetTransparent](./settransparent/) | Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Gibt an, ob die Schriftart eines Zeichens nur ersetzt werden soll, wenn die Zellen-Schriftart nicht kompatibel ist. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Gibt an, ob die Schriftart eines Zeichens nur ersetzt werden soll, wenn die Zellen-Schriftart nicht kompatibel ist. |
| [SetPageIndex](./setpageindex/) | Liest oder setzt den nullbasierten Index der ersten zu speichernden Seite. |
| [GetPageIndex](./getpageindex/) | Liest oder setzt den nullbasierten Index der ersten zu speichernden Seite. |
| [SetPageCount](./setpagecount/) | Liest oder setzt die Anzahl der zu speichernden Seiten. |
| [GetPageCount](./getpagecount/) | Liest oder setzt die Anzahl der zu speichernden Seiten. |
| [SetDesiredSize](./setdesiredsize/) | Setzt die gewünschte Breite und Höhe des Bildes. |
| [IsOptimized](./isoptimized/) | Gibt an, ob die Ausgabeelemente optimiert werden sollen. |
| [SetIsOptimized](./setisoptimized/) | Gibt an, ob die Ausgabeelemente optimiert werden sollen. |
| [GetDefaultFont](./getdefaultfont/) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie in PDF/Bild als Block erscheinen. Setzen Sie die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode-Zeichen anzuzeigen. |
| [SetDefaultFont](./setdefaultfont/) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie in PDF/Bild als Block erscheinen. Setzen Sie die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode-Zeichen anzuzeigen. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie in PDF/Bild als Block erscheinen. Setzen Sie dies auf true, um zunächst zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie in PDF/Bild als Block erscheinen. Setzen Sie dies auf true, um zunächst zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [GetGridlineType](./getgridlinetype/) | Liest oder setzt den Rasterlinientyp. |
| [SetGridlineType](./setgridlinetype/) | Liest oder setzt den Rasterlinientyp. |
| [GetGridlineColor](./getgridlinecolor/) | Liest oder setzt die Farbe der Rasterlinien. |
| [SetGridlineColor](./setgridlinecolor/) | Liest oder setzt die Farbe der Rasterlinien. |
| [GetTextCrossType](./gettextcrosstype/) | Liest oder legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [SetTextCrossType](./settextcrosstype/) | Liest oder legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Liest oder legt die Standardsprache für die Bearbeitung fest. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Liest oder legt die Standardsprache für die Bearbeitung fest. |
| [GetSheetSet](./getsheetset/) | Liest oder legt die zu rendernden Arbeitsblätter fest. Standard ist: Alle sichtbaren Arbeitsblätter in der Arbeitsmappe: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Liest oder legt die zu rendernden Arbeitsblätter fest. Standard ist: Alle sichtbaren Arbeitsblätter in der Arbeitsmappe: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Einstellung für das Rendern von EMF-Metadateien in der Quelldatei. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Einstellung für das Rendern von EMF-Metadateien in der Quelldatei. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Liest oder legt benutzerdefinierte Einstellungen während des Renderns fest. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Liest oder legt benutzerdefinierte Einstellungen während des Renderns fest. |
