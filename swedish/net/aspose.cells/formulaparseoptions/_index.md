---
title: "Klass FormulaParseOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FormulaParseOptions klass. Representerar alternativ när formel analyseras"
type: docs
url: /sv/net/aspose.cells/formulaparseoptions/
---
## FormulaParseOptions class

Representerar alternativ när formel analyseras.

```csharp
public class FormulaParseOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [FormulaParseOptions](formulaparseoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CheckAddIn](../../aspose.cells/formulaparseoptions/checkaddin/) { get; set; } | Om tillägg ska kontrolleras i befintliga externa länkar i den aktuella arbetsboken för användardefinierade funktioner utan extern länk. Standard är true (om en användardefinierad funktion matchar ett tillägg i befintliga externa länkar, tas det som tillägget). |
| [CustomFunctionDefinition](../../aspose.cells/formulaparseoptions/customfunctiondefinition/) { get; set; } | Definition för att analysera anpassade funktioner. |
| [LocaleDependent](../../aspose.cells/formulaparseoptions/localedependent/) { get; set; } | Om formeln är lokalanpassad. Standard är false. |
| [Parse](../../aspose.cells/formulaparseoptions/parse/) { get; set; } | Om given formel ska analyseras. Standard är true. Om den är false, behålls formelsträngen oförändrad i cellen tills användaren anropar andra metoder för att analysera den eller analyserad formeldatat behövs för andra operationer såsom beräkning av formler. |
| [R1C1Style](../../aspose.cells/formulaparseoptions/r1c1style/) { get; set; } | Om formeln använder R1C1-referensstil. Standard är false. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaParseOptionsDemo
    {
        public static void FormulaParseOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false,
                CheckAddIn = true,
                Parse = true,
                CustomFunctionDefinition = null // Assuming no custom function definition for this example
            };

            // Lägg till en formel i en cell med hjälp av alternativen
            Cell cell = worksheet.Cells["A1"];
            cell.SetFormula("=SUM(B1:B10)", options);

            // Spara arbetsboken
            workbook.Save("FormulaParseOptionsExample.xlsx");
            workbook.Save("FormulaParseOptionsExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


