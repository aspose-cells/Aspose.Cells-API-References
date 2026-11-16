---
title: "AboveAverage Klasse"
linktitle: "AboveAverage"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "AboveAverage Klasse. Kapselt das Objekt, das aboveaverage in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/aboveaverage/
---

## AboveAverage class

Beschreiben Sie die AboveAverage‑Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel hebt Zellen hervor, die über oder unter dem Durchschnitt aller Werte im Bereich liegen.

```go

type AboveAverage struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewAboveAverage](./newaboveaverage/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [IsAboveAverage](./isaboveaverage/) | Abrufen oder Festlegen des Flags, das angibt, ob die Regel eine „überdurchschnittliche“ Regel ist. 'true' bedeutet 'überdurchschnittlich'. Standardwert ist true. |
| [SetIsAboveAverage](./setisaboveaverage/) | Abrufen oder Festlegen des Flags, das angibt, ob die Regel eine „überdurchschnittliche“ Regel ist. 'true' bedeutet 'überdurchschnittlich'. Standardwert ist true. |
| [IsEqualAverage](./isequalaverage/) | Abrufen oder Festlegen des Flags, das angibt, ob die Kriterien 'aboveAverage' und 'belowAverage' den Durchschnittswert einschließen oder ausschließen. 'true' bedeutet, den Durchschnittswert in die Kriterien einzubeziehen. Standardwert ist false. |
| [SetIsEqualAverage](./setisequalaverage/) | Abrufen oder Festlegen des Flags, das angibt, ob die Kriterien 'aboveAverage' und 'belowAverage' den Durchschnittswert einschließen oder ausschließen. 'true' bedeutet, den Durchschnittswert in die Kriterien einzubeziehen. Standardwert ist false. |
| [GetStdDev](./getstddev/) | Abrufen oder Festlegen der Anzahl der Standardabweichungen, die über oder unter dem Durchschnitt in der bedingten Formatierungsregel berücksichtigt werden sollen. Der Eingabewert muss zwischen 0 und 3 liegen (einschließlich 0 und 3). Das Setzen dieses Werts auf 0 bedeutet, dass stdDev nicht festgelegt ist. Der Standardwert ist 0. |
| [SetStdDev](./setstddev/) | Abrufen oder Festlegen der Anzahl der Standardabweichungen, die über oder unter dem Durchschnitt in der bedingten Formatierungsregel berücksichtigt werden sollen. Der Eingabewert muss zwischen 0 und 3 liegen (einschließlich 0 und 3). Das Setzen dieses Werts auf 0 bedeutet, dass stdDev nicht festgelegt ist. Der Standardwert ist 0. |
