---
title: "Worksheet.CalculateFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Beräknar en formel"
type: docs
url: /sv/net/aspose.cells/worksheet/calculateformula/
---
## CalculateFormula(string) {#calculateformula}

Beräknar en formel.

```csharp
public object CalculateFormula(string formula)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formel att beräkna. |

### Returvärde

Beräknat formelresultat.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];

            // Demonstrera grundläggande talomvandling
            string formula = "=NUMBERVALUE(\"1.234\")";
            Console.WriteLine("NUMBERVALUE(\"1.234\") = " + sheet.CalculateFormula(formula));

            // Demonstrera valutakonvertering
            formula = "=NUMBERVALUE(\"$1,234.56\")";
            Console.WriteLine("NUMBERVALUE(\"$1,234.56\") = " + sheet.CalculateFormula(formula));

            // Demonstrera tidsomvandling
            formula = "=NUMBERVALUE(\"0:25\")";
            Console.WriteLine("NUMBERVALUE(\"0:25\") = " + sheet.CalculateFormula(formula));

            // Demonstrera datumomvandling
            formula = "=NUMBERVALUE(\"07/26/2023\")";
            Console.WriteLine("NUMBERVALUE(\"07/26/2023\") = " + sheet.CalculateFormula(formula));

            // Demonstrera felscenario
            formula = "=NUMBERVALUE(\"invalid\")";
            Console.WriteLine("NUMBERVALUE(\"invalid\") = " + sheet.CalculateFormula(formula));
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, CalculationOptions) {#calculateformula_1}

Beräknar ett formeluttryck direkt.

```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formel att beräkna. |
| opts | CalculationOptions | Alternativ för att beräkna formel |

### Returvärde

Beräknat resultat av given formel. Det returnerade objektet kan vara av möjliga typer av [`Value`](../../cell/value/), eller ReferredArea.

### Anmärkningar

Formeln kommer att beräknas precis som den har satts i cell A1. Och formeln kommer att behandlas som en normal formel. Om du behöver att formeln beräknas som en matrisformel och få en matris för det beräknade resultatet, använd [`CalculateArrayFormula`](../calculatearrayformula/) istället.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Skapa en anpassad beräkningsmotor
            CustomEngine customEngine = new CustomEngine();
            
            // Beräkna formel med anpassad motor
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };
            
            object result = worksheet.CalculateFormula("=SUM(A1:A3)", options);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object value = data.GetParamValue(i);
                    if (value is double)
                    {
                        sum += (double)value;
                    }
                }
                data.CalculatedValue = sum;
            }
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

## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}

Beräknar ett formeluttryck direkt.

```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts, 
    int baseCellRow, int baseCellColumn, CalculationData calculationData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formel att beräkna. |
| pOpts | FormulaParseOptions | Alternativ för att tolka formel. |
| cOpts | CalculationOptions | Alternativ för att beräkna formel. |
| baseCellRow | Int32 | Radindex för bascellen. |
| baseCellColumn | Int32 | Kolumnindex för bascellen. |
| calculationData | CalculationData | Beräkningsdata. Den används i situationer där användaren behöver beräkna vissa statiska formler när en anpassad beräkningsmotor implementeras. För sådana situationer måste användaren specificera den med beräkningsdata som tillhandahålls för [`Calculate`](../../abstractcalculationengine/calculate/). |

### Returvärde

Beräknat resultat av given formel. Det returnerade objektet kan vara av möjliga typer av [`Value`](../../cell/value/), eller ReferredArea.

### Anmärkningar

Formeln kommer att beräknas precis som den har ställts in på den angivna bascellen. Och formeln kommer att tas som en normal formel. Om du behöver att formeln beräknas som en matrisformel och få en matris för det beräknade resultatet, använd [`CalculateArrayFormula`](../calculatearrayformula/) istället.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringFormulaParseOptCalculati169472Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i exempeldata
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C1"].PutValue(2);
            worksheet.Cells["C2"].PutValue(4);

            // Definiera beräkningsalternativ
            CalculationOptions calculationOptions = new CalculationOptions();
            
            // Definiera alternativ för formelparsning
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions();
            
            // Beräkna formel med alla parametrar
            object result = worksheet.CalculateFormula(
                "=SUM(B1:B2, C1:C2)",  // formula
                formulaParseOptions,   // parse options
                calculationOptions,    // calculation options
                0,                     // base cell row
                0,                     // base cell column
                null                   // calculation data
            );

            // Skriv ut resultatet
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Se även

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}

Beräknar alla formler i detta kalkylblad.

```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | CalculationOptions | Alternativ för beräkning |
| rekursiv | Boolean | Sant betyder att om kalkylbladets celler är beroende av celler i andra kalkylblad, så kommer de beroende cellerna i de andra kalkylbladen också att beräknas. Falskt betyder att alla formler i kalkylbladet har beräknats och värdena är korrekta. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithCalculationOptionsBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempeldata och formler
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue("=SUM(A1:A3)");
            
            // Skapa beräkningsalternativ
            CalculationOptions options = new CalculationOptions();
            options.Recursive = true;
            options.IgnoreError = false;
            
            // Beräkna formel med alternativ och tvinga fullständig beräkning
            worksheet.CalculateFormula(options, true);
            
            // Skriv ut det beräknade resultatet
            Console.WriteLine("Calculated value: " + worksheet.Cells["B1"].StringValue);
        }
    }
}
```

### Se även

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


