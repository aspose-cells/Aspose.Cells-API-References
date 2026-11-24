---
title: "Cell.IsErrorValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Prüft, ob der Wert dieser Zelle ein Fehler ist."
type: docs
url: /de/net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

Überprüft, ob der Wert dieser Zelle ein Fehler ist.

```csharp
public bool IsErrorValue { get; }
```

### Hinweise

Gilt auch für Formelfelder, um zu prüfen, ob das berechnete Ergebnis ein Fehler ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsErrorValueDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzen Sie eine Formel, die zu einem Fehler führt.
            Cell cell = cells["A1"];
            cell.Formula = "=1/0"; // Division by zero error
            
            // Formeln berechnen
            workbook.CalculateFormula();

            // Demonstration der IsErrorValue‑Eigenschaft
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("IsErrorValue: " + cell.IsErrorValue);
            Console.WriteLine("Error type: " + cell.Value);

            // Setzen Sie einen gültigen Wert.
            Cell cell2 = cells["A2"];
            cell2.PutValue("Valid value");
            
            Console.WriteLine("\nCell A2 value: " + cell2.StringValue);
            Console.WriteLine("IsErrorValue: " + cell2.IsErrorValue);

            // Setzen Sie einen SPILL-Fehler (Excel 365+ Dynamisches Array‑Formelfehler).
            Cell cell3 = cells["A3"];
            cell3.SetDynamicArrayFormula("=A1:A10", new FormulaParseOptions(), true);
            
            Console.WriteLine("\nCell A3 value: " + cell3.StringValue);
            Console.WriteLine("IsErrorValue: " + cell3.IsErrorValue);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


