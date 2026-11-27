---
title: "Cell.FormulaLocal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämta den lokalanpassade formeln för cellen"
type: docs
url: /sv/net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

Hämta den lokalanpassade formeln för cellen.

```csharp
public string FormulaLocal { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaLocalDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in standardlokal till tyska för demonstration
            workbook.Settings.Region = CountryCode.Germany;
            
            // Åtkomst till cell A1
            Cell cell = worksheet.Cells["A1"];
            
            // Ange formel i standardformat (engelska)
            cell.Formula = "=SUM(B1:C1)";
            
            // Visa formler i både standard- och lokala format
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Ange formel i lokalt format (tyska)
            cell.FormulaLocal = "=SUMME(B1:C1)";
            
            // Visa formler igen för att visa skillnaden
            Console.WriteLine("\nAfter setting FormulaLocal:");
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Demonstrera GetFormula med lokalisering
            Console.WriteLine("\nUsing GetFormula:");
            Console.WriteLine("English formula: " + cell.GetFormula(false, false));
            Console.WriteLine("Localized formula: " + cell.GetFormula(false, true));
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


