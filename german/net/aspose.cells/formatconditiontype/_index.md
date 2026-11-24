---
title: "Enum FormatConditionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FormatConditionType-Enum. Typ der bedingten Formatierungsregel"
type: docs
url: /de/net/aspose.cells/formatconditiontype/
---
## FormatConditionType enumeration

Bedingter Formatregeltyp.

```csharp
public enum FormatConditionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| CellValue | `1` | Diese bedingte Formatierungsregel vergleicht den Wert einer Zelle mit einem durch eine Formel berechneten Ergebnis unter Verwendung eines Operators. |
| Expression | `2` | Diese bedingte Formatierungsregel enthält eine zu bewertende Formel. Wenn das Formel-Ergebnis wahr ist, wird die Zelle hervorgehoben. |
| Top10 | `4` | Diese bedingte Formatierungsregel hebt Zellen hervor, deren Werte in das obere N‑ oder untere N‑Intervall fallen, wie angegeben. |
| UniqueValues | `8` | Diese bedingte Formatierungsregel hebt eindeutige Werte im Bereich hervor. |
| DuplicateValues | `16` | Diese bedingte Formatierungsregel hebt duplizierte Werte hervor. |
| ContainsText | `32` | Diese bedingte Formatierungsregel hebt Zellen hervor, die den angegebenen Text enthalten. Entspricht der Verwendung der SEARCH()-Tabellenfunktion, um zu bestimmen, ob die Zelle den Text enthält. |
| NotContainsText | `64` | Diese bedingte Formatierungsregel hebt Zellen hervor, die den angegebenen Text nicht enthalten. Entspricht der Verwendung der SEARCH()-Tabellenfunktion, um zu bestimmen, ob die Zelle den Text enthält oder nicht. |
| BeginsWith | `128` | Diese bedingte Formatierungsregel hebt Zellen im Bereich hervor, die mit dem angegebenen Text beginnen. Entspricht der Verwendung der LEFT()-Tabellenfunktion und dem Vergleich der Werte. |
| EndsWith | `256` | Diese bedingte Formatierungsregel hebt Zellen hervor, die mit dem angegebenen Text enden. Entspricht der Verwendung der RIGHT()-Tabellenfunktion und dem Vergleich der Werte. |
| ContainsBlanks | `512` | Diese bedingte Formatierungsregel hebt Zellen hervor, die vollständig leer sind. Entspricht der Verwendung von LEN(TRIM()). Das bedeutet, dass wenn die Zelle nur Zeichen enthält, die TRIM() entfernen würde, sie als leer gilt. Eine leere Zelle wird ebenfalls als leer betrachtet. |
| NotContainsBlanks | `1024` | Diese bedingte Formatierungsregel hebt Zellen hervor, die nicht leer sind. Entspricht der Verwendung von LEN(TRIM()). Das bedeutet, dass wenn die Zelle nur Zeichen enthält, die TRIM() entfernen würde, sie als leer gilt. Eine leere Zelle wird ebenfalls als leer betrachtet. |
| ContainsErrors | `2048` | Diese bedingte Formatierungsregel hebt Zellen mit Formelfehlern hervor. Entspricht der Verwendung der ISERROR()-Tabellenfunktion, um zu bestimmen, ob ein Formelfehler vorliegt. |
| NotContainsErrors | `4096` | Diese bedingte Formatierungsregel hebt Zellen ohne Formelfehler hervor. Entspricht der Verwendung der ISERROR()-Tabellenfunktion, um zu bestimmen, ob ein Formelfehler vorliegt. |
| TimePeriod | `8192` | Diese bedingte Formatierungsregel hebt Zellen hervor, die Daten im angegebenen Zeitraum enthalten. Der zugrunde liegende Wert der Zelle wird ausgewertet, daher muss die Zelle nicht als Datum formatiert sein, um ausgewertet zu werden. Zum Beispiel wird bei einer Zelle mit dem Wert 38913 die bedingte Formatierung angewendet, wenn die Regel einen Wert von 7/14/2006 erfordert. |
| AboveAverage | `16384` | Diese bedingte Formatierungsregel hebt Zellen hervor, die über oder unter dem Durchschnitt aller Werte im Bereich liegen. |
| ColorScale | `32768` | Diese bedingte Formatierungsregel erstellt eine abgestufte Farbskala auf den Zellen. |
| DataBar | `65536` | Diese bedingte Formatierungsregel zeigt eine abgestufte Datenleiste im Zellbereich an. |
| IconSet | `131072` | Diese bedingte Formatierungsregel wendet Symbole auf Zellen entsprechend ihrer Werte an. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionTypeDemo
    {
        public static void FormatConditionTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch.
            Workbook workbook = new Workbook();

            // Hole das erste Arbeitsblatt.
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügt eine leere bedingte Formatierung hinzu
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Setzt den Bereich für die bedingte Formatierung.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Fügt eine Bedingung für AboveAverage hinzu
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Einstellen von Eigenschaften für AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Fügt eine Bedingung für CellValue hinzu
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // Fügt eine Bedingung für ContainsText hinzu
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = "Sample";
            fc3.Style.BackgroundColor = Color.Green;

            // Speichere die Excel-Datei
            workbook.Save("FormatConditionTypeExample.xlsx");
            workbook.Save("FormatConditionTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


