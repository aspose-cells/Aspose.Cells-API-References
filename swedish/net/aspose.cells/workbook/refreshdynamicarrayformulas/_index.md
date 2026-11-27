---
title: "Workbook.RefreshDynamicArrayFormulas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Uppdaterar dynamisk array‑formelspill till ett nytt område av intilliggande celler enligt aktuell data. Andra formler i arbetsboken kommer inte att beräknas rekursivt även om de användes av dynamiska array‑formler"
type: docs
url: /sv/net/aspose.cells/workbook/refreshdynamicarrayformulas/
---
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}

Uppdaterar dynamiska matrisformler(sprider sig till ett nytt område av intilliggande celler enligt aktuell data) Andra formler i arbetsboken kommer inte att beräknas rekursivt även om de användes av dynamiska matrisformler.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| beräkna | Boolean | Om den beräknar och uppdaterar cellvärden för dessa dynamiska array‑formler |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet1 = wb.Worksheets[0];
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");

            // Ställ in initial data och dynamiska array‑formler
            sheet1.Cells["A1"].PutValue("B1:B3");
            sheet1.Cells["A2"].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), true);
            sheet2.Cells["B1"].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!A2#)", new FormulaParseOptions(), true);

            Console.WriteLine("Before refresh:");
            PrintSpillStatus(sheet1, sheet2);

            // Ändra området och uppdatera formler
            sheet1.Cells["A1"].PutValue("B1:B5");
            wb.RefreshDynamicArrayFormulas(true);

            Console.WriteLine("\nAfter refresh:");
            PrintSpillStatus(sheet1, sheet2);
        }

        private static void PrintSpillStatus(Worksheet sheet1, Worksheet sheet2)
        {
            Console.WriteLine("Sheet1 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet1.Cells.CheckCell(i, 0);
                Console.WriteLine($"Row {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }

            Console.WriteLine("\nSheet2 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet2.Cells.CheckCell(0, i);
                Console.WriteLine($"Column {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}

Uppdaterar dynamiska matrisformler(sprider sig till ett nytt område av intilliggande celler enligt aktuell data)

```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| beräkna | Boolean | Om den beräknar och uppdaterar cellvärden för dessa dynamiska array‑formler |
| copts | CalculationOptions | Alternativen för att beräkna formler |

### Anmärkningar

Av prestandaskäl uppdaterar vi inte automatiskt alla dynamiska array‑formler när själva formeln eller de data den refererar till ändras. Därför måste användaren anropa den här metoden manuellt efter de operationer som kan påverka dynamiska array‑formler, såsom import/inställning av cellvärden, infogning/ta bort rader/kolumner/områden, …etc. För de flesta formler med funktioner krävs beräkning av spill‑området också beräkning av formeln, så i allmänhet föredras ett sant värde för flaggan "calculate". Om formeln är enkel, till exempel en områdesreferens eller array (t.ex. "=C1:E5", "={1,2;3,4}", …), enkel funktion på ett område eller array (t.ex. "=ABS(C1:E5)", "=1+{1,2;3,4}", …), och alla formler kommer att beräknas senare (t.ex. via [`CalculateFormula`](../calculateformula/)), kan ett falskt värde för flaggan "calculate" undvika duplicerad beräkning till fördel för prestandan.

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanCalculationOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempel på dynamisk array‑formel
            worksheet.Cells["A1"].Formula = "=SEQUENCE(5)";
            
            // Skapa beräkningsalternativ
            CalculationOptions opts = new CalculationOptions();
            opts.CalcStackSize = 100;
            
            // Uppdatera dynamiska array‑formler med beräkningsalternativ
            workbook.RefreshDynamicArrayFormulas(true, opts);
            
            // Beräkna arbetsbokens formler
            workbook.CalculateFormula(opts);
            
            // Skriv ut resultatet från A1:A5
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].Value);
            }
        }
    }
}
```

### Se även

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


