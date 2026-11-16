---
title: "ErrorCheckType‑Enum"
linktitle: "ErrorCheckType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ErrorCheckType‑Enum. Kapselt das Objekt, das errorchecktype in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/errorchecktype/
---

## ErrorCheckType Enum

Stellt alle Fehlertypen für die Prüfung dar.

```go

type ErrorCheckType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [EvaluationError](./evaluationerror/) | Ignoriere Fehler, wenn Zellen Formeln enthalten, die einen Fehler ergeben. |
| [EmptyCellRef](./emptycellref/) | Ignoriere Fehler, wenn Formeln sich auf leere Zellen beziehen. |
| [NumberStoredAsText](./numberstoredastext/) | Ignoriere Fehler, wenn Zahlen als Text formatiert sind oder von einem Apostroph vorangestellt werden |
| [InconsistRange](./inconsistrange/) | Ignoriere Fehler, wenn Formeln bestimmte Zellen in einem Bereich weglassen. |
| [InconsistFormula](./inconsistformula/) | Ignoriere Fehler, wenn eine Formel in einem Bereich Ihres Arbeitsblatts von anderen Formeln im selben Bereich abweicht. |
| [TwoDigitTextYear](./twodigittextyear/) | Ignoriere Fehler, wenn Formeln Textzellen mit zweistellig dargestellten Jahren enthalten. |
| [UnlockedFormula](./unlockedformula/) | Ignoriere Fehler, wenn nicht gesperrte Zellen Formeln enthalten. |
| [TableDataValidation](./tabledatavalidation/) | Ignoriere Fehler, wenn der Zellenwert in einer Tabelle nicht den angegebenen Datenvalidierungsregeln entspricht. |
| [CalculatedColumn](./calculatedcolumn/) | Ignoriere Fehler, wenn Zellen einen von einer berechneten Spaltenformel abweichenden Wert enthalten. |
