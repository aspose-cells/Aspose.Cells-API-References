---
title: "Validation.SetFormula2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validierungsmethode. Legt den Wert oder Ausdruck fest, der mit dieser Validierung verknüpft ist"
type: docs
url: /de/net/aspose.cells/validation/setformula2/
---
## Validation.SetFormula2 method

Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class ValidationMethodSetFormula2WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielreferenzwerte einfügen
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["B1"].PutValue(200);

            // Datenvalidierung für Zelle C1 erstellen
            ValidationCollection validations = worksheet.Validations;
            Validation validation = validations[validations.Add()];
            validation.AddArea(CellArea.CreateCellArea(0, 0, 2, 2)); // Applies to cell C1

            // Validierungsparameter konfigurieren
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.ShowError = true;
            validation.ErrorTitle = "Range Error";
            validation.ErrorMessage = "Value must be between A1 (100) and B1 (200)";

            try
            {
                // Setze Validierungsformeln unter Verwendung der erforderlichen Parametertypen
                validation.SetFormula1("=A1", false, false);
                validation.SetFormula2("=B1", false, false); // Demonstrate (String, Boolean, Boolean)

                Console.WriteLine("SetFormula2 executed successfully with formula '=B1'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("ValidationSetFormula2Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


