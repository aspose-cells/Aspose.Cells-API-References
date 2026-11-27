---
title: "Workbook.UpdateCustomFunctionDefinition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Uppdaterar definitionen av anpassade funktioner"
type: docs
url: /sv/net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

Uppdaterar definitionen av anpassade funktioner.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| definition | CustomFunctionDefinition | Speciell definition av anpassade funktioner för användarens speciella krav. |

### Anmärkningar

Denna metod kan användas för vissa speciella scenarier. Till exempel, om användaren behöver vissa parametrar för anpassade funktioner beräknas i array‑läge, kan användaren tillhandahålla sin egen definition med implementerad [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) för dessa funktioner. Efter att formeldata har uppdaterats kommer de angivna parametrarna automatiskt att beräknas i array‑läge när motsvarande anpassade funktioner beräknas.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["B1"].PutValue(1);
            sheet.Cells["C1"].PutValue(2);
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["C2"].PutValue(8);

            // Skapa anpassad beräkningsmotor
            var customEngine = new MyCustomCalculationEngine();
            
            // Ställ in beräkningsalternativ med anpassad motor
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };

            // Uppdatera definitionen av den anpassade funktionen
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());

            // Ange formel med anpassad funktion
            sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
            
            // Beräkna formler
            wb.CalculateFormula(options);

            // Skriv ut resultatet
            Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
        }
    }

    public class MyCustomFunctionDefinition : CustomFunctionDefinition
    {
        public override int[] GetArrayModeParameters(string functionName)
        {
            // Returnera parameterindex som ska behandlas i array‑läge
            return new int[] { 0 }; // First parameter is array mode
        }
    }

    public class MyCustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYFUNC")
            {
                double sum = 0;
                var paramValue = data.GetParamValue(0);
                
                if (paramValue is object[,] arrayValue)
                {
                    foreach (var val in arrayValue)
                    {
                        if (val != null)
                        {
                            sum += Convert.ToDouble(val);
                        }
                    }
                }
                else
                {
                    sum += Convert.ToDouble(paramValue);
                }
                data.CalculatedValue = sum * 2; // Custom calculation logic
            }
        }
    }
}
```

### Se även

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


