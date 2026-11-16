---
title: "SplitPartInfo Klasse"
linktitle: "SplitPartInfo"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SplitPartInfo Klasse. Kapselt das Objekt, das splitpartinfo in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/splitpartinfo/
---

## SplitPartInfo class

Stellt die Informationen eines Eingabe-/Ausgabe-Paares für mehrere Eingaben/Ausgaben dar, z. B. die aktuelle Seite, die beim Konvertieren einer Tabellenkalkulation in ein Bild gerendert werden soll.

```go

type SplitPartInfo struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetPartIndex](./getpartindex/) | Index des aktuellen Teils in der Sequenz (0-basiert). -1 bedeutet, dass es keine mehreren Teile gibt, sodass das Ergebnis einzeln ist. |
| [GetSheetIndex](./getsheetindex/) | Index des Blatts, in dem sich der aktuelle Teil befindet. -1 bedeutet, dass es nur ein Blatt gibt. |
| [GetSheetName](./getsheetname/) | Name des Blatts, in dem sich der aktuelle Teil befindet. |
