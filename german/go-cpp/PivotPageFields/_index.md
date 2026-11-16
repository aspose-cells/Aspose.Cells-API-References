---
title: "PivotPageFields Klasse"
linktitle: "PivotPageFields"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotPageFields Klasse. Kapselt das Objekt, das PivotPageFields in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivotpagefields/
---

## PivotPageFields class

Stellt die Pivot‑Seiten‑Elemente dar, wenn die Datenquelle der Pivot‑Tabelle Konsolidierungsbereiche ist. Sie kann höchstens 4 Elemente enthalten.

```go

type PivotPageFields struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewPivotPageFields](./newpivotpagefields/) | Stellt die Pivot‑Seitenfeld‑Elemente dar. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [AddPageField](./addpagefield/) | Fügt ein Seitenfeld hinzu. |
| [GetPageFieldCount](./getpagefieldcount/) | Ermittelt die Anzahl der Seitenfelder. |
| [AddIdentify](./addidentify/) | Legt fest, welches Elementlabel in jedem Seitenfeld zur Identifizierung des Datenbereichs verwendet wird. Die pageItemIndex.Length muss gleich PageFieldCount sein, bitte fügen Sie zuerst das Seitenfeld hinzu. |
