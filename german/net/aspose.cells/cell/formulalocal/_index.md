---
title: "Cell.FormulaLocal"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Zelleneigenschaft. Gibt die lokalisierte formatierte Formel der Zelle zurück"
type: docs
url: /de/net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

Liefert die lokalisierte formatierte Formel der Zelle.

```csharp
public string FormulaLocal { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaLocalDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Standard-Locale für die Demonstration auf Deutsch setzen
            workbook.Settings.Region = CountryCode.Germany;
            
            // Zugriff auf Zelle A1
            Cell cell = worksheet.Cells["A1"];
            
            // Formel im Standardformat (Englisch) festlegen
            cell.Formula = "=SUM(B1:C1)";
            
            // Formeln sowohl im Standard- als auch im lokalen Format anzeigen
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Formel im lokalen Format (Deutsch)
            cell.FormulaLocal = "=SUMME(B1:C1)";
            
            // Formeln erneut anzeigen, um den Unterschied zu zeigen
            Console.WriteLine("\nAfter setting FormulaLocal:");
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // GetFormula mit Lokalisierung demonstrieren
            Console.WriteLine("\nUsing GetFormula:");
            Console.WriteLine("English formula: " + cell.GetFormula(false, false));
            Console.WriteLine("Localized formula: " + cell.GetFormula(false, true));
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


