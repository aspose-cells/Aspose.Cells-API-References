---
title: "Cell.SetDynamicArrayFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Anger dynamisk arrayformel och låter formeln spilla över till närliggande celler om möjligt"
type: docs
url: /sv/net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | String | formeluttrycket |
| alternativ | FormulaParseOptions | alternativ för att tolka formel. Alternativet "Parse" kommer att ignoreras och formeln kommer alltid att tolkas omedelbart |
| calculateValue | Boolean | om den dynamiska arrayformeln ska beräknas för de celler i det spillade området. |

### Returvärde

det område som formeln ska spilla in i.

### Anmärkningar

det returnerade området kan skilja sig från det faktiska området som denna dynamiska arrayformel spillar in i. Om det finns icke-tomma celler i området kommer formeln att sättas endast för den aktuella cellen och markeras som "#SPILL!". Men i en sådan situation returnerar vi fortfarande hela området som formeln ska spilla in i.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsBooleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ange dynamisk arrayformel i cell A1
            Cell cell1 = cells["A1"];
            cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);

            // Ange värde i B2 som kommer att påverka SEQUENCE-formeln
            cells["B2"].PutValue(3);

            // Beräkna formler och uppdatera dynamiska arrayer
            wb.CalculateFormula();
            wb.RefreshDynamicArrayFormulas(false);

            // Skriv ut resultaten från det spillade området
            Console.WriteLine("Dynamic array results:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine(cells[0, i].Value);
            }
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | String | formeluttrycket |
| alternativ | FormulaParseOptions | alternativ för att tolka formel. Alternativet "Parse" kommer att ignoreras och formeln kommer alltid att tolkas omedelbart |
| värden | Object[][] | values(beräknade resultat) för de celler med given dynamisk array-formel |
| calculateRange | Boolean | Om den spillda området ska beräknas för denna dynamiska array-formel. Om parametern "values" inte är null och denna flagga är falsk, kommer den spillda områdets höjd att vara values.Length och bredden att vara values[0].Length. |
| calculateValue | Boolean | om denna dynamiska array-formel ska beräknas för de celler i det spillda området när "values" är null eller motsvarande element i "values" för en cell är null. |

### Returvärde

det område som formeln ska spilla in i.

### Anmärkningar

det returnerade området kan skilja sig från det faktiska området som denna dynamiska arrayformel spillar in i. Om det finns icke-tomma celler i området kommer formeln att sättas endast för den aktuella cellen och markeras som "#SPILL!". Men i en sådan situation returnerar vi fortfarande hela området som formeln ska spilla in i.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue(10);
            cell = cells["A2"];
            cell.PutValue(20);
            cell = cells["B1"];
            cell.PutValue(60);
            cell = cells["B2"];
            cell.PutValue(80);

            // Hämta cell C1 där den dynamiska array-formeln ska sättas
            cell = worksheet.Cells["C1"];

            // Definiera den dynamiska array-formeln
            string formula = "=A1:B2 * 2";
            
            // Skapa alternativ för formelparsning
            FormulaParseOptions options = new FormulaParseOptions
            {
                Parse = true // Enable formula parsing
            };

            // Förbered values för att fylla i cellerna med formelresultat
            object[][] values = new object[2][];
            values[0] = new object[] { 2, 4 };
            values[1] = new object[] { 6, 8 };

            try
            {
                // Ange dynamisk array-formel med förberäknade values
                CellArea result = cell.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange: false,  // Use values array dimensions for spill range
                    calculateValue: false  // Use provided values instead of calculating
                );

                Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
            }

            // Spara arbetsboken med ändringarna
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}

Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | String | formeluttrycket |
| alternativ | FormulaParseOptions | alternativ för att tolka formel. Alternativet "Parse" kommer att ignoreras och formeln kommer alltid att tolkas omedelbart |
| värden | Object[][] | values(beräknade resultat) för de celler med given dynamisk array-formel |
| calculateRange | Boolean | Om den spillda området ska beräknas för denna dynamiska array-formel. Om parametern "values" inte är null och denna flagga är falsk, kommer den spillda områdets höjd att vara values.Length och bredden att vara values[0].Length. |
| calculateValue | Boolean | om denna dynamiska array-formel ska beräknas för de celler i det spillda området när "values" är null eller motsvarande element i "values" för en cell är null. |
| copts | CalculationOptions | Alternativen för att beräkna formeln. Vanligtvis, med hänsyn till prestanda, bör egenskapen [`Recursive`](../../calculationoptions/recursive/) vara falsk. |

### Returvärde

det område som formeln ska spilla in i.

### Anmärkningar

det returnerade området kan skilja sig från det faktiska området som denna dynamiska arrayformel spillar in i. Om det finns icke-tomma celler i området kommer formeln att sättas endast för den aktuella cellen och markeras som "#SPILL!". Men i en sådan situation returnerar vi fortfarande hela området som formeln ska spilla in i.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata i cellerna A2:B5
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B3"].PutValue(55);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["B5"].PutValue(70);

            // Hämta målcell D1
            Cell cellD1 = worksheet.Cells["D1"];

            try
            {
                // Förbered parametrar för SetDynamicArrayFormula
                string formula = "=FILTER(A2:A5, B2:B5>50)";
                FormulaParseOptions options = new FormulaParseOptions { Parse = true };
                object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
                bool calculateRange = true;
                bool calculateValue = true;
                CalculationOptions calcOptions = new CalculationOptions { Recursive = true };

                // Anropa SetDynamicArrayFormula med specifika parametrar
                CellArea spillRange = cellD1.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange,
                    calculateValue,
                    calcOptions
                );

                Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


