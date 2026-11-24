---
title: "FormulaParseOptions.CustomFunctionDefinition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaParseOptions Eigenschaft. Definition zum Parsen benutzerdefinierter Funktionen"
type: docs
url: /de/net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

Definition zum Parsen benutzerdefinierter Funktionen.

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### Hinweise

Für einige spezielle Anforderungen, wie zum Beispiel beim Berechnen einer benutzerdefinierten Funktion in der benutzerdefinierten Engine des Benutzers, müssen einige ihrer Parameter im Array-Modus berechnet werden; mit dieser Eigenschaft können diese Parameter beim Parsen der Formel als Array-Modus markiert werden. Andernfalls muss der Benutzer diese benutzerdefinierten Funktionen später mit [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) aktualisieren, um das gleiche Ergebnis zu erhalten.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Benutzerdefinierte Funktionsdefinition erstellen
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
            
            // Formel-Parse-Optionen mit benutzerdefinierter Funktion einrichten
            FormulaParseOptions options = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunction,
                Parse = true
            };

            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);

            // Benutzerdefinierte Funktion in Formel verwenden
            string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
            worksheet.Cells["C1"].SetFormula(formula, options);

            // Arbeitsmappe berechnen, um die Verarbeitung benutzerdefinierter Funktionen zu demonstrieren
            workbook.CalculateFormula();

            // Ergebnis speichern
            workbook.Save("CustomFunctionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


