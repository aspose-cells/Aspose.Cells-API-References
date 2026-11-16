---
title: "LoadFilter-Klasse"
linktitle: "LoadFilter"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "LoadFilter-Klasse. Kapselt das Objekt, das loadfilter in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/loadfilter/
---

## LoadFilter class

Stellt den Filter dar, der Optionen zum Laden von Daten beim Laden einer Arbeitsmappe aus einer Vorlage bereit.

```go

type LoadFilter struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewLoadFilter](./newloadfilter/) | Erstellt einen LoadFilter mit den Standardfilteroptionen LoadDataFilterOptions::All. |
| [NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | Erstellt einen LoadFilter mit den angegebenen Filteroptionen. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetLoadDataFilterOptions](./getloaddatafilteroptions/) | Liest die Filteroptionen, um anzugeben, welche Daten geladen werden sollen. |
| [SetLoadDataFilterOptions](./setloaddatafilteroptions/) | Setzt die Filteroptionen, um anzugeben, welche Daten geladen werden sollen. |
| [GetSheetsInLoadingOrder](./getsheetsinloadingorder/) | Gibt die zu ladenden Blätter (Indizes) und deren Reihenfolge an. Standard ist null, was bedeutet, dass alle Blätter in der Standardreihenfolge der Vorlagendatei geladen werden. Ist der Wert nicht null und ist der Index eines Blattes nicht im zurückgegebenen Array enthalten, wird dieses Blatt nicht geladen. |
| [StartSheet](./startsheet/) | Bereitet die Filteroptionen vor dem Laden des angegebenen Arbeitsblatts vor. Die Implementierung von LoadFilter durch den Benutzer kann die LoadDataFilterOptions ändern, um festzulegen, wie Daten für dieses Arbeitsblatt geladen werden. |
