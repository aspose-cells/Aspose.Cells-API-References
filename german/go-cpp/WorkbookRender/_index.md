---
title: "WorkbookRender-Klasse"
linktitle: "WorkbookRender"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "WorkbookRender-Klasse. Kapselt das Objekt, das workbookrender in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/workbookrender/
---

## WorkbookRender class

Stellt ein Arbeitsmappen-Rendern dar. Der Konstruktor dieser Klasse muss nach Änderungen des Seitenlayouts und des Zellstils verwendet werden.

```go

type WorkbookRender struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewWorkbookRender](./newworkbookrender/) | Der Aufbau von WorkbookRender |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetPageCount](./getpagecount/) | Ermittelt die Gesamtseitenzahl des Arbeitsbuchs. |
| [GetPageSizeInch](./getpagesizeinch/) | Ermittelt die Seitengröße in Zoll des Ausgabebildes. |
| [ToImage](./toimage/) | Rendern des gesamten Arbeitsbuchs als Tiff-Bild in einen Stream. |
| [ToImage_String](./toimage_string/) | Rendern des gesamten Arbeitsbuchs als Tiff-Bild in eine Datei. |
| [ToImage_Int_String](./toimage_int_string/) | Rendern einer bestimmten Seite in eine Datei. |
| [ToImage_Int](./toimage_int/) | Rendern einer bestimmten Seite in einen Stream. |
| [Dispose](./dispose/) | Gibt Ressourcen frei, die für das Rendern erstellt und verwendet wurden. |
