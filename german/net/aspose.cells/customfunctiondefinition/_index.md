---
title: "Klasse CustomFunctionDefinition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CustomFunctionDefinition Klasse. Definition einer benutzerdefinierten Funktion für Berechnungen mit einer benutzerdefinierten Engine."
type: docs
url: /de/net/aspose.cells/customfunctiondefinition/
---
## CustomFunctionDefinition class

Definition einer benutzerdefinierten Funktion zur Berechnung mit der benutzerdefinierten Engine des Benutzers.

```csharp
public class CustomFunctionDefinition
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | Der Standardkonstruktor. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | Liest die Indizes der Parameter der angegebenen benutzerdefinierten Funktion, die im Arraymodus berechnet werden müssen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionDemo
    {
        public static void CustomFunctionDefinitionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle eine neue Instanz von CustomFunctionDefinition
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // Erstellen Sie eine neue FormulaParseOptions-Instanz und setzen Sie die CustomFunctionDefinition
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // Fügen Sie dem Arbeitsbuch ein Arbeitsblatt hinzu
            Worksheet worksheet = workbook.Worksheets[0];

            // Definieren Sie eine benutzerdefinierte Formel
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // Analysieren Sie die benutzerdefinierte Formel mit den FormulaParseOptions
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


