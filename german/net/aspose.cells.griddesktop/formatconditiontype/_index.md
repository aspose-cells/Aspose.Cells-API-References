---
title: "Enum FormatConditionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.FormatConditionType-Aufzählung. Typ der bedingten Formatierungsregel."
type: docs
url: /de/net/aspose.cells.griddesktop/formatconditiontype/
---
## FormatConditionType enumeration

Bedingter Formatregeltyp.

```csharp
public enum FormatConditionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| CellValue | `0` | Diese bedingte Formatierungsregel vergleicht den Wert einer Zelle mit einem durch eine Formel berechneten Ergebnis unter Verwendung eines Operators. |
| Expression | `1` | Diese bedingte Formatierungsregel enthält eine zu bewertende Formel. Wenn das Formel-Ergebnis wahr ist, wird die Zelle hervorgehoben. |
| ColorScale | `2` | Diese bedingte Formatierungsregel erstellt eine abgestufte Farbskala auf den Zellen. |
| DataBar | `3` | Diese bedingte Formatierungsregel zeigt eine abgestufte Datenleiste im Zellbereich an. |
| IconSet | `4` | Diese bedingte Formatierungsregel wendet Symbole auf Zellen entsprechend ihrer Werte an. |
| Top10 | `5` | Diese bedingte Formatierungsregel hebt Zellen hervor, deren Werte in das obere N‑ oder untere N‑Intervall fallen, wie angegeben. |
| UniqueValues | `6` | Diese bedingte Formatierungsregel hebt eindeutige Werte im Bereich hervor. |
| DuplicateValues | `7` | Diese bedingte Formatierungsregel hebt duplizierte Werte hervor. |
| ContainsText | `8` | Diese bedingte Formatierungsregel hebt Zellen hervor, die den angegebenen Text enthalten. Entspricht der Verwendung der SEARCH()-Tabellenfunktion, um zu bestimmen, ob die Zelle den Text enthält. |
| NotContainsText | `9` | Diese bedingte Formatierungsregel hebt Zellen hervor, die nicht leer sind. Entspricht der Verwendung von LEN(TRIM()). Das bedeutet, dass wenn die Zelle nur Zeichen enthält, die TRIM() entfernen würde, sie als leer gilt. Eine leere Zelle wird ebenfalls als leer betrachtet. |
| BeginsWith | `10` | Diese bedingte Formatierungsregel hebt Zellen im Bereich hervor, die mit dem angegebenen Text beginnen. Entspricht der Verwendung der LEFT()-Tabellenfunktion und dem Vergleich der Werte. |
| EndsWith | `11` | Diese bedingte Formatierungsregel hebt Zellen hervor, die mit dem angegebenen Text enden. Entspricht der Verwendung der RIGHT()-Tabellenfunktion und dem Vergleich der Werte. |
| ContainsBlanks | `12` | Diese bedingte Formatierungsregel hebt Zellen hervor, die vollständig leer sind. Entspricht der Verwendung von LEN(TRIM()). Das bedeutet, dass wenn die Zelle nur Zeichen enthält, die TRIM() entfernen würde, sie als leer gilt. Eine leere Zelle wird ebenfalls als leer betrachtet. |
| NotContainsBlanks | `13` | Diese bedingte Formatierungsregel hebt Zellen hervor, die nicht leer sind. Entspricht der Verwendung von LEN(TRIM()). Das bedeutet, dass wenn die Zelle nur Zeichen enthält, die TRIM() entfernen würde, sie als leer gilt. Eine leere Zelle wird ebenfalls als leer betrachtet. |
| ContainsErrors | `14` | Diese bedingte Formatierungsregel hebt Zellen mit Formelfehlern hervor. Entspricht der Verwendung der ISERROR()-Tabellenfunktion, um zu bestimmen, ob ein Formelfehler vorliegt. |
| NotContainsErrors | `15` | Diese bedingte Formatierungsregel hebt Zellen ohne Formelfehler hervor. Entspricht der Verwendung der ISERROR()-Tabellenfunktion, um zu bestimmen, ob ein Formelfehler vorliegt. |
| TimePeriod | `16` | Diese bedingte Formatierungsregel hebt Zellen hervor, die Daten im angegebenen Zeitraum enthalten. Der zugrunde liegende Wert der Zelle wird ausgewertet, daher muss die Zelle nicht als Datum formatiert sein, um ausgewertet zu werden. Zum Beispiel wird bei einer Zelle mit dem Wert 38913 die bedingte Formatierung angewendet, wenn die Regel einen Wert von 7/14/2006 erfordert. |
| AboveAverage | `17` | Diese bedingte Formatierungsregel hebt Zellen hervor, die über oder unter dem Durchschnitt aller Werte im Bereich liegen. |

### Siehe auch

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


