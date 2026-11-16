---
title: "FormatConditionType Aufzählung"
linktitle: "FormatConditionType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "FormatConditionType Aufzählung. Kapselt das Objekt, das formatconditiontype in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/formatconditiontype/
---

## FormatConditionType Enum

Typ der bedingten Formatierungsregel.

```go

type FormatConditionType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [CellValue](./cellvalue/) | Diese bedingte Formatierungsregel vergleicht einen Zellenwert mit einem durch eine Formel berechneten Ergebnis, wobei ein Operator verwendet wird. |
| [Expression](./expression/) | Diese bedingte Formatierungsregel enthält eine zu bewertende Formel. Wenn das Formelresultat wahr ist, wird die Zelle hervorgehoben. |
| [Top10](./top10/) | Diese bedingte Formatierungsregel hebt Zellen hervor, deren Werte in das obere N‑ oder untere N‑Intervall fallen, wie angegeben. |
| [UniqueValues](./uniquevalues/) | Diese bedingte Formatierungsregel hebt eindeutige Werte im Bereich hervor. |
| [DuplicateValues](./duplicatevalues/) | Diese bedingte Formatierungsregel hebt duplizierte Werte hervor. |
| [ContainsText](./containstext/) | Diese bedingte Formatierungsregel hebt Zellen hervor, die den angegebenen Text enthalten. Entspricht der Verwendung der SEARCH()-Tabellenfunktion, um zu bestimmen, ob die Zelle den Text enthält. |
| [NotContainsText](./notcontainstext/) | Diese bedingte Formatierungsregel hebt Zellen hervor, die den angegebenen Text nicht enthalten. Entspricht der Verwendung der SEARCH()-Tabellenfunktion, um zu bestimmen, ob die Zelle den Text enthält oder nicht. |
| [BeginsWith](./beginswith/) | Diese bedingte Formatierungsregel hebt Zellen im Bereich hervor, die mit dem angegebenen Text beginnen. Entspricht der Verwendung der LEFT()-Tabellenfunktion und dem Vergleich der Werte. |
| [EndsWith](./endswith/) | Diese bedingte Formatierungsregel hebt Zellen hervor, die mit dem angegebenen Text enden. Entspricht der Verwendung der RIGHT()-Tabellenfunktion und dem Vergleich der Werte. |
| [ContainsBlanks](./containsblanks/) | Diese bedingte Formatierungsregel hebt Zellen hervor, die vollständig leer sind. Entspricht der Verwendung von LEN(TRIM()). Das bedeutet, dass wenn die Zelle nur Zeichen enthält, die TRIM() entfernen würde, sie als leer betrachtet wird. Eine leere Zelle wird ebenfalls als leer betrachtet. |
| [NotContainsBlanks](./notcontainsblanks/) | Diese bedingte Formatierungsregel hebt Zellen hervor, die nicht leer sind. Entspricht der Verwendung von LEN(TRIM()). Das bedeutet, dass wenn die Zelle nur Zeichen enthält, die TRIM() entfernen würde, sie als leer betrachtet wird. Eine leere Zelle wird ebenfalls als leer betrachtet. |
| [ContainsErrors](./containserrors/) | Diese bedingte Formatierungsregel hebt Zellen mit Formelfehlern hervor. Entspricht der Verwendung der ISERROR()-Tabellenfunktion, um zu bestimmen, ob ein Formelfehler vorliegt. |
| [NotContainsErrors](./notcontainserrors/) | Diese bedingte Formatierungsregel hebt Zellen ohne Formelfehler hervor. Entspricht der Verwendung der ISERROR()-Tabellenfunktion, um zu bestimmen, ob ein Formelfehler vorliegt. |
| [TimePeriod](./timeperiod/) | Diese bedingte Formatierungsregel hebt Zellen hervor, die Daten im angegebenen Zeitraum enthalten. Der zugrunde liegende Wert der Zelle wird ausgewertet, daher muss die Zelle nicht als Datum formatiert sein, um ausgewertet zu werden. Zum Beispiel wird bei einer Zelle mit dem Wert 38913 die bedingte Formatierung angewendet, wenn die Regel einen Wert vom 14.07.2006 erfordert. |
| [AboveAverage](./aboveaverage/) | Diese bedingte Formatierungsregel hebt Zellen hervor, die über oder unter dem Durchschnitt aller Werte im Bereich liegen. |
| [ColorScale](./colorscale/) | Diese bedingte Formatierungsregel erstellt eine abgestufte Farbskala in den Zellen. |
| [DataBar](./databar/) | Diese bedingte Formatierungsregel zeigt eine abgestufte Datenleiste im Zellbereich an. |
| [IconSet](./iconset/) | Diese bedingte Formatierungsregel wendet Symbole auf Zellen basierend auf deren Werten an. |
