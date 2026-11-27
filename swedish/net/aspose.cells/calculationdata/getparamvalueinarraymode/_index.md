---
title: "CalculationData.GetParamValueInArrayMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData method. Hämtar värdena för parametern vid ett givet index. Om parametern är någon form av uttryck som måste beräknas, beräknas den i arrayläge."
type: docs
url: /sv/net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Hämtar värdet/värdena för parametern på ett givet index. Om parametern är någon form av uttryck som måste beräknas, beräknas den i arrayläge.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Index för parametern (0‑baserat) |
| maxRowCount | Int32 | Radräkningsgränsen för den returnerade arrayen. Om den är noll eller negativ eller större än det faktiska antalet rader, används det faktiska antalet rader. |
| maxColumnCount | Int32 | Kolumnräkningsgränsen för den returnerade arrayen. Om den är noll eller negativ eller större än det faktiska antalet kolumner, används det faktiska antalet kolumner. |

### Returvärde

En array som innehåller alla objekt som representeras av den angivna parametern.

### Anmärkningar

För ett uttryck som måste beräknas, med A:A+B:B som exempel: I värdeläge beräknas det till ett enda värde enligt den aktuella cellens bas. Men i arrayläge beräknas alla värden för A1+B1,A2+B2,A3+B3,... och används för att konstruera den returnerade arrayen. I sådana situationer är det bättre att ange gränsen för rad‑/kolumnantalet (t.ex. enligt [`MaxDataRow`](../../cells/maxdatarow/) och [`MaxDataColumn`](../../cells/maxdatacolumn/)), annars kan den stora returnerade arrayen öka minneskostnaden med en stor mängd oanvänd data.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för sammanhang
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // Skapa beräkningsalternativ med anpassad motor
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // Anropa GetParamValueInArrayMode med realistiska parametrar
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
                }
            }
        }
    }
}
```

### Se även

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


