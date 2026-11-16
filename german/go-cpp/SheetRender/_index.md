---
title: "SheetRender Klasse"
linktitle: "SheetRender"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SheetRender Klasse. Kapselt das Objekt, das sheetrender in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/sheetrender/
---

## SheetRender class

Stellt ein Arbeitsblatt-Rendern dar, das das Arbeitsblatt in verschiedene Bilder wie (BMP, PNG, JPEG, TIFF…) rendern kann. Der Konstruktor dieser Klasse muss nach Änderungen der Seitenlayout‑Einstellungen und des Zellstils verwendet werden.

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewSheetRender](./newsheetrender/) | Der Konstruktor von SheetRender benötigt worksheet und ImageOrPrintOptions als Parameter. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetPageCount](./getpagecount/) | Liefert die Gesamtseitenzahl des aktuellen Arbeitsblatts. |
| [GetPageScale](./getpagescale/) | Liefert den berechneten Seitenskalierungsfaktor des Blatts. Gibt die eingestellte Skalierung zurück, wenn PageSetup.Zoom gesetzt ist. Andernfalls wird die berechnete Skalierung gemäß PageSetup.FitToPagesWide und PageSetup.FitToPagesTall zurückgegeben. |
| [GetPageSizeInch](./getpagesizeinch/) | Ermittelt die Seitengröße in Zoll des Ausgabebildes. |
| [ToImage_Int_String](./toimage_int_string/) | Rendern einer bestimmten Seite in eine Datei. |
| [ToImage_Int](./toimage_int/) | Rendern einer bestimmten Seite in einen Stream. |
| [ToTiff](./totiff/) | Rendert das gesamte Arbeitsblatt als Tiff-Bild in einen Stream. |
| [ToTiff_String](./totiff_string/) | Rendert das gesamte Arbeitsblatt als Tiff-Bild in eine Datei. |
| [Dispose](./dispose/) | Gibt Ressourcen frei, die für das Rendern erstellt und verwendet wurden. |
