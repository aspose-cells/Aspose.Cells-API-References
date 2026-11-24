---
title: "Enum ErrorCheckType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ErrorCheckType enum. Stellt alle Fehlprüfungsarten dar"
type: docs
url: /de/net/aspose.cells/errorchecktype/
---
## ErrorCheckType enumeration

Stellt alle Fehlerprüfungsarten dar.

```csharp
public enum ErrorCheckType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| EvaluationError | `1` | Ignoriere Fehler, wenn Zellen Formeln enthalten, die einen Fehler ergeben. |
| Calc | `1` |  |
| EmptyCellRef | `2` | Ignoriere Fehler, wenn Formeln sich auf leere Zellen beziehen. |
| NumberStoredAsText | `4` | Ignoriere Fehler, wenn Zahlen als Text formatiert sind oder von einem Apostroph vorangestellt werden |
| TextNumber | `4` | Ignoriere Fehler, wenn Zahlen als Text formatiert sind oder von einem Apostroph vorangestellt werden |
| InconsistRange | `8` | Ignoriere Fehler, wenn Formeln bestimmte Zellen in einem Bereich weglassen. |
| InconsistFormula | `16` | Ignoriere Fehler, wenn eine Formel in einem Bereich Ihres Arbeitsblatts von anderen Formeln im selben Bereich abweicht. |
| TwoDigitTextYear | `32` | Ignoriere Fehler, wenn Formeln Textzellen enthalten, in denen Jahre als zweistellige Zahlen dargestellt werden. |
| TextDate | `32` | Ignoriere Fehler, wenn Formeln Textzellen enthalten, in denen Jahre als zweistellige Zahlen dargestellt werden. |
| UnlockedFormula | `64` | Ignoriere Fehler, wenn nicht gesperrte Zellen Formeln enthalten. |
| UnproctedFormula | `64` | Ignoriere Fehler, wenn nicht gesperrte Zellen Formeln enthalten. |
| TableDataValidation | `128` | Ignoriere Fehler, wenn der Wert einer Zelle in einer Tabelle nicht den angegebenen Datenvalidierungsregeln entspricht. |
| Validation | `128` | Ignoriere Fehler, wenn der Wert einer Zelle in einer Tabelle nicht den angegebenen Datenvalidierungsregeln entspricht. |
| CalculatedColumn | `129` | Ignoriere Fehler, wenn Zellen einen Wert enthalten, der von einer berechneten Spaltenformel abweicht. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckTypeDemo
    {
        public static void ErrorCheckTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf die ErrorCheckOptionCollection zu
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Füge eine neue ErrorCheckOption hinzu
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            // Setze verschiedene Fehlprüfungsarten auf false
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);

            // Definiere einen Zellbereich für die ErrorCheckOption
            CellArea cellArea = CellArea.CreateCellArea("A1", "B10");
            errorCheckOption.AddRange(cellArea);

            // Speichere die Arbeitsmappe
            workbook.Save("ErrorCheckTypeExample.xlsx");
            workbook.Save("ErrorCheckTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


