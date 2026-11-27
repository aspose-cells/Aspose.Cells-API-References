---
title: "Klass AbstractCalculationEngine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AbstractCalculationEngine-klass. Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells"
type: docs
url: /sv/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells.

```csharp
public abstract class AbstractCalculationEngine
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | Anger om denna motor behöver parametern beräknas i array‑läge. Standardvärdet är falskt. Om [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) krävs vid beräkning av anpassade funktioner och användaren inte har uppdaterat definitionen för dem (med [`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/)), ska denna egenskap sättas till true. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | Anger om denna motor behöver den bokstavliga texten för parametern under en beräkning. Standardvärdet är falskt. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | Om inbyggda funktioner som stöds av den inbyggda motorn ska kontrolleras och bearbetas av denna implementation. Standard är falskt. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | Beräknar en funktion med angivna data. |
| virtual [ForceRecalculate](../../aspose.cells/abstractcalculationengine/forcerecalculate/)(string) | Om den angivna funktionen ska tvingas att alltid beräknas om vid beräkning av delade formler. |
| [SkipCalculation](../../aspose.cells/abstractcalculationengine/skipcalculation/)() | Hoppar över beräkningen för hela formeln som refererar till funktionen som för närvarande utvärderas. |

### Anmärkningar

Användaren bör inte ändra någon del av Workbook direkt i denna implementation (förutom det beräknade resultatet av den anpassade funktionen, som kan sättas via egenskapen CalculationData.CalculatedValue). Annars kan oväntade resultat eller ett Exception uppstå. Om användaren behöver ändra annan data än det beräknade resultatet i implementationen för vissa anpassade funktioner, till exempel ändra cellens formel, stil, …etc., bör användaren samla dessa data i implementationen och ändra dem utanför formelberäkningens område.

### Exempel

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Exempel: Anpassad implementation för en funktion med namnet "MYFUNC"
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // Antag att MYFUNC tar två parametrar och returnerar deras summa
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            // Tvinga omberäkning för den anpassade funktionen "MYFUNC"
            return functionName.ToUpper() == "MYFUNC";
        }
    }

    public class CalculationEngineDemo
    {
        public static void Test()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Placera några värden i celler
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);

            // Lägg till en formel som använder den anpassade funktionen
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";

            // Ställ in beräkningsalternativ med den anpassade motorn
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = new CustomCalculationEngine(),
                IgnoreError = false,
                Recursive = true
            };

            // Beräkna formler med den anpassade motorn
            workbook.CalculateFormula(options);

            // Skriv ut resultatet av den anpassade funktionen
            Console.WriteLine("Result of MYFUNC(A1, A2): " + sheet.Cells["A3"].Value);

            // Spara arbetsboken
            workbook.Save("CustomCalculationEngineExample.xlsx");
            workbook.Save("CustomCalculationEngineExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


