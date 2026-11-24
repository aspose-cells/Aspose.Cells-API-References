---
title: "Klasse FormulaParseOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FormulaParseOptions Klasse. Stellt Optionen beim Parsen von Formeln dar"
type: docs
url: /de/net/aspose.cells/formulaparseoptions/
---
## FormulaParseOptions class

Stellt Optionen beim Parsen von Formeln dar.

```csharp
public class FormulaParseOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FormulaParseOptions](formulaparseoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CheckAddIn](../../aspose.cells/formulaparseoptions/checkaddin/) { get; set; } | Ob Add‑Ins in bestehenden externen Links der aktuellen Arbeitsmappe für benutzerdefinierte Funktionen ohne externen Link überprüft werden sollen. Standard ist true (wenn die benutzerdefinierte Funktion mit einem Add‑In in bestehenden externen Links übereinstimmt, wird sie als dieses Add‑In betrachtet). |
| [CustomFunctionDefinition](../../aspose.cells/formulaparseoptions/customfunctiondefinition/) { get; set; } | Definition zum Parsen benutzerdefinierter Funktionen. |
| [LocaleDependent](../../aspose.cells/formulaparseoptions/localedependent/) { get; set; } | Ob die Formel lokalisierungsformatiert ist. Standard ist false. |
| [Parse](../../aspose.cells/formulaparseoptions/parse/) { get; set; } | Ob die gegebene Formel geparst werden soll. Standard ist true. Wenn sie false ist, bleibt die Formelzeichenkette unverändert in der Zelle, bis der Benutzer andere Methoden zum Parsen aufruft oder geparste Formeldaten von anderen Vorgängen wie der Berechnung von Formeln benötigt werden. |
| [R1C1Style](../../aspose.cells/formulaparseoptions/r1c1style/) { get; set; } | Ob die Formel im R1C1-Bezugsstil vorliegt. Standard ist false. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaParseOptionsDemo
    {
        public static void FormulaParseOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false,
                CheckAddIn = true,
                Parse = true,
                CustomFunctionDefinition = null // Assuming no custom function definition for this example
            };

            // Füge einer Zelle eine Formel mit den Optionen hinzu
            Cell cell = worksheet.Cells["A1"];
            cell.SetFormula("=SUM(B1:B10)", options);

            // Speichere die Arbeitsmappe
            workbook.Save("FormulaParseOptionsExample.xlsx");
            workbook.Save("FormulaParseOptionsExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


