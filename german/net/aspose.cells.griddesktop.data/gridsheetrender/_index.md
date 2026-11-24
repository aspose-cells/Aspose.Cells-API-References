---
title: "Class GridSheetRender"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.Data.GridSheetRender class. Stellt eine Arbeitsblattdarstellung dar, die ein Arbeitsblatt in verschiedene Bilder wie BMP, PNG, JPEG, TIFF usw. rendern kann. Der Konstruktor dieser Klasse muss nach der Änderung des Seitenlayouts der Zellenstil verwendet werden."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridsheetrender/
---
## GridSheetRender class

Stellt ein Arbeitsblatt‑Rendern dar, das das Arbeitsblatt in verschiedene Bilder wie (BMP, PNG, JPEG, TIFF…) rendern kann. Der Konstruktor dieser Klasse muss nach der Änderung von pagesetup und cell style verwendet werden.

```csharp
public class GridSheetRender
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | Der Konstruktor von SheetRender benötigt ein Arbeitsblatt und ImageOrPrintOptions als Parameter |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | Gibt die Gesamtseitenzahl des aktuellen Arbeitsblatts zurück. |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | Ermittelt den berechneten Seitenskalierungsfaktor des Blatts. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | Ermittelt die Seitengröße in Zoll des Ausgabebildes. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | Rendert eine bestimmte Seite in ein Bitmap-Objekt. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | Rendert eine bestimmte Seite in einen Stream. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | Rendert eine bestimmte Seite in eine Datei. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Bestimmte Seite in ein Graphics-Objekt rendern |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Bestimmte Seite in ein Graphics-Objekt rendern |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | Arbeitsblatt zum Drucker rendern |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | Arbeitsblatt zum Drucker rendern |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Arbeitsblatt zum Drucker rendern |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | Arbeitsblatt zum Drucker rendern |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | Ganzes Arbeitsblatt als Tiff‑Bild in einen Stream rendern. |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | Ganzes Arbeitsblatt als Tiff‑Bild in eine Datei rendern. |

### Siehe auch

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


