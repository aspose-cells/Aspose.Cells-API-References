---
title: "ColumnCollection-Klasse"
linktitle: "ColumnCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ColumnCollection-Klasse. Kapselt das Objekt, das columncollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/columncollection/
---

## ColumnCollection class

Sammlung der <see cref=\"Column\"/>-Objekte, die die einzelnen Spalten(einstellungen) in einem Arbeitsblatt darstellen. Das Column‑Objekt repräsentiert nur Einstellungen wie Spaltenbreite, Stile usw. für die gesamte Spalte und hat nichts damit zu tun, ob in der entsprechenden Spalte nicht‑leere Zellen (Daten) vorhanden sind oder nicht. Und die \"Count\"‑Eigenschaft dieser Sammlung gibt nur die Anzahl der Column‑Objekte an, die in dieser Sammlung instanziiert wurden, und hat ebenfalls nichts damit zu tun, ob im Arbeitsblatt nicht‑leere Zellen (Daten) vorhanden sind oder nicht.

```go

type ColumnCollection struct  {
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
| [GetColumnByIndex](./getcolumnbyindex/) | Liest das Column‑Objekt anhand seiner Position in der Liste. |
| [Get](./get/) | Liest ein Column‑Objekt anhand des Spaltenindex. Das Column‑Objekt des angegebenen Spaltenindex wird erstellt, falls es vorher nicht existiert. |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
