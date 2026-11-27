---
title: "Worksheet.CalculateArrayFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Beräknar en formel som matrisformel"
type: docs
url: /sv/net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

Beräknar en formel som matrisformel.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formel att beräkna. |
| opts | CalculationOptions | Alternativ för att beräkna formel |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite exempeldata
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Definiera en matrisformel
            string arrayFormula = "=SUM(A1:B3)";
            
            // Beräkna matrisformeln med beräkningsalternativ
            object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
            
            // Skriv ut resultatet
            Console.WriteLine("Result of array formula calculation: " + result[0][0]);
        }
    }
}
```

### Se även

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

Beräknar en formel som matrisformel.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formel att beräkna. |
| opts | CalculationOptions | Alternativ för att beräkna formel |
| maxRowCount | Int32 | det maximala antalet rader i resulterande data. Om det är noll eller negativt eller större än det faktiska antalet rader, kommer det faktiska antalet rader att användas. |
| maxColumnCount | Int32 | det maximala antalet kolumner i resulterande data. Om det är noll eller negativt eller större än det faktiska antalet rader, kommer det faktiska antalet kolumner att användas. |

### Returvärde

Beräknat formelresultat.

### Anmärkningar

Formeln kommer att tas som en dynamisk matrisformel för att beräkna dimensionen och resultatet. Användarspecificerad maximal dimension används för fall där det beräknade resultatet är en stor datamängd (till exempel kan det beräknade resultatet motsvara en hel rad- eller kolumndata) men användaren inte behöver så stor en matris enligt affärskrav eller av prestandaskäl.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exempel 1: Enkel beräkning av matrisformel
            string formula = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions options = new CalculationOptions();
            object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);

            // Exempel 2: Matrisformel med dynamiskt område
            formula = "=LEN(IF({1;2;3;4},B2:B5))";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);

            // Exempel 3: Matrisformel med MATCH-funktionen
            // Skapa lite testdata
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(10);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["C3"].PutValue(2);
            sheet.Cells["D2"].PutValue(0);
            sheet.Cells["D3"].PutValue(0);

            formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of MATCH formula: " + result[0][0]);
        }
    }
}
```

### Se även

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

Beräknar en formel som matrisformel.

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formel att beräkna. |
| pOpts | FormulaParseOptions | Alternativ för att tolka formel |
| cOpts | CalculationOptions | Alternativ för att beräkna formel |
| baseCellRow | Int32 | Radindex för bascellen. |
| baseCellColumn | Int32 | Kolumnindex för bascellen. |
| maxRowCount | Int32 | Det maximala antalet rader i resulterande data. Om det är noll eller negativt eller större än det faktiska antalet rader, kommer det faktiska antalet rader att användas. |
| maxColumnCount | Int32 | Det maximala antalet kolumner i resulterande data. Om det är noll eller negativt eller större än det faktiska antalet rader, kommer det faktiska antalet kolumner att användas. |
| calculationData | CalculationData | Beräkningsdata. Den används i situationer där användaren behöver beräkna vissa statiska formler när en anpassad beräkningsmotor implementeras. För sådana situationer måste användaren specificera den med beräkningsdata som tillhandahålls för [`Calculate`](../../abstractcalculationengine/calculate/). |

### Returvärde

Beräknat formelresultat.

### Anmärkningar

Formeln kommer att tas som en dynamisk matrisformel för att beräkna dimensionen och resultatet. Användarspecificerad maximal dimension används för fall där det beräknade resultatet är en stor datamängd (till exempel kan det beräknade resultatet motsvara en hel rad- eller kolumndata) men användaren inte behöver så stor en matris enligt affärskrav eller av prestandaskäl.

### Se även

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


