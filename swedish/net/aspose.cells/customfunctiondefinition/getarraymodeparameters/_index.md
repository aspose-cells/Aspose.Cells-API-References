---
title: "CustomFunctionDefinition.GetArrayModeParameters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomFunctionDefinition-metod. Hämtar indexen för angivna anpassade funktionsparametrar som måste beräknas i array‑läge"
type: docs
url: /sv/net/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---
## CustomFunctionDefinition.GetArrayModeParameters method

Hämtar indexen för den angivna anpassade funktionens parametrar som måste beräknas i arrayläge.

```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionName | String | Namnet på den anpassade funktionen. |

### Returvärde

Index för parametrarna som måste beräknas i array‑läge för given anpassad funktion. Standard är null, det finns ingen parameter som måste beräknas i array‑läge för den anpassade funktionen.

### Anmärkningar

För ett uttryck som måste beräknas, med A:A+B:B som exempel: Vanligtvis i värdeläge beräknas det till ett enda värde enligt den aktuella cellbasen. Men i array‑läge beräknas alla värden av A1+B1, A2+B2, A3+B3, … och används för beräkningen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av CustomFunctionDefinition
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();

            try
            {
                // Anropa GetArrayModeParameters med ett funktionsnamnsparameter
                string functionName = "SUM";
                int[] result = customFunction.GetArrayModeParameters(functionName);

                // Visa resultatet
                if (result != null)
                {
                    Console.WriteLine("Array mode parameters for function '{0}':", functionName);
                    foreach (int param in result)
                    {
                        Console.WriteLine(param);
                    }
                }
                else
                {
                    Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
        }
    }
}
```

### Se även

* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


