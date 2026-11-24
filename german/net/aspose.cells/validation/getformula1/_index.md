---
title: "Validation.GetFormula1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validierungsmethode. Gibt den Wert oder Ausdruck zurück, der mit dieser Validierung verknüpft ist"
type: docs
url: /de/net/aspose.cells/validation/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Liest den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Rückgabewert

Der Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula1WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Validierung zur ersten Zelle hinzu
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Validierung auf Zelle A1 anwenden
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // Rufe GetFormula1 mit den Parametern (false, false) auf, um die Formel in A1-Notation zu erhalten
                string formula1 = validation.GetFormula1(false, false);
                
                Console.WriteLine("Formula1 in A1 notation: " + formula1);
                
                // Rufen Sie GetFormula1 mit den Parametern (true, false) auf, um die Formel in R1C1-Notation zu erhalten.
                string formula1R1C1 = validation.GetFormula1(true, false);
                
                Console.WriteLine("Formula1 in R1C1 notation: " + formula1R1C1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ValidationMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Liest den Wert oder Ausdruck, der mit dieser Validierung für eine bestimmte Zelle verknüpft ist.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Rückgabewert

Der Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula1WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Validierung in Zelle B5 (Zeile 4, Spalte 1).
            CellArea area = CellArea.CreateCellArea(4, 1, 4, 1); // Use static method via type name
            int validationIndex = worksheet.Validations.Add(area); // Get validation index
            Validation validation = worksheet.Validations[validationIndex]; // Retrieve validation object
            validation.Type = ValidationType.Custom;
            validation.Formula1 = "=A5"; // Relative reference to cell A5

            try
            {
                // Rufen Sie GetFormula1 mit dem R1C1-Format für Zelle B5 auf.
                string formulaR1C1 = validation.GetFormula1(true, false, 4, 1);
                Console.WriteLine($"R1C1 Formula: {formulaR1C1}");

                // Rufen Sie GetFormula1 mit dem A1-Format für Zelle B5 auf.
                string formulaA1 = validation.GetFormula1(false, false, 4, 1);
                Console.WriteLine($"A1 Formula: {formulaA1}");

                workbook.Save("ValidationGetFormula1Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


