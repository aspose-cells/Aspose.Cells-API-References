---
title: "Klasse ErrorCheckOption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ErrorCheckOption Klasse. Fehlerprüfungs‑Einstellung, die auf bestimmte Bereiche angewendet wird"
type: docs
url: /de/net/aspose.cells/errorcheckoption/
---
## ErrorCheckOption class

Fehlerprüfungs‑Einstellung, die auf bestimmte Bereiche angewendet wird.

```csharp
public class ErrorCheckOption
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | Fügt einen von dieser Einstellung beeinflussten Bereich hinzu. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | Ermittelt die Anzahl der von dieser Einstellung beeinflussten Bereiche. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | Ermittelt den von dieser Einstellung beeinflussten Bereich anhand des angegebenen Index. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | Prüft, ob der angegebene Fehlertyp überprüft wird. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | Entfernt einen Bereich anhand des angegebenen Index. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | Legt fest, ob der angegebene Fehlertyp überprüft wird. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionDemo
    {
        public static void ErrorCheckOptionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die ErrorCheckOptionCollection vom Arbeitsblatt ab
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // Füge der Sammlung eine neue ErrorCheckOption hinzu
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // Fehlerprüfungsoptionen festlegen
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // Definiere einen Zellbereich und füge ihn zur ErrorCheckOption hinzu
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // Speichere die Arbeitsmappe
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


