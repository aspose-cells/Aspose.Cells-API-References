---
title: "Validation.SetFormula1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validierungsmethode. Legt den Wert oder Ausdruck fest, der mit dieser Validierung verknüpft ist"
type: docs
url: /de/net/aspose.cells/validation/setformula1/
---
## Validation.SetFormula1 method

Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| isR1C1 | Boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | Boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten in Zelle B1 vorbereiten
            worksheet.Cells["B1"].PutValue(100);

            // Datenvalidierung für Zelle A1 erstellen
            int validationIndex = worksheet.Validations.Add(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.Decimal;
            validation.Operator = OperatorType.GreaterOrEqual;
            validation.ShowError = true;
            validation.ErrorTitle = "Validation Error";
            validation.ErrorMessage = "Value must be greater than or equal to cell B1 (100)";

            try
            {
                // Formel festlegen, die B1 mit A1-Notation referenziert (nicht R1C1, nicht lokal)
                validation.SetFormula1("=B1", false, false);
                Console.WriteLine("SetFormula1 executed successfully with parameters (String, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1: {ex.Message}");
            }

            // Arbeitsmappe mit Validierung speichern
            workbook.Save("ValidationSetFormula1Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


