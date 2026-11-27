---
title: "CellsHelper.GetDateTimeFromDouble"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Konvertera dubbelvärdet till datum‑tidsvärdet"
type: docs
url: /sv/net/aspose.cells/cellshelper/getdatetimefromdouble/
---
## CellsHelper.GetDateTimeFromDouble method

Konvertera dubbelvärdet till datum‑tidsvärdet.

```csharp
public static DateTime GetDateTimeFromDouble(double doubleValue, bool date1904)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| doubleValue | Double | Det dubbla värdet. |
| date1904 | Boolean | 1904-datumsystem. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetDateTimeFromDoubleWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered data för metodparametrarna (Double, Boolean)
            double doubleValue = 44197.5; // Represents 2021-01-01 12:00:00 in Excel serial date format
            bool date1904 = false; // Using 1900 date system

            try
            {
                // Anropa GetDateTimeFromDouble‑metoden med de specifika parametertyperna
                DateTime result = CellsHelper.GetDateTimeFromDouble(doubleValue, date1904);
                
                // Visa resultatet
                Console.WriteLine($"Converted DateTime: {result}");
                
                // Skriv resultatet till en cell
                worksheet.Cells["A1"].PutValue("Original Double Value:");
                worksheet.Cells["B1"].PutValue(doubleValue);
                worksheet.Cells["A2"].PutValue("Converted DateTime:");
                worksheet.Cells["B2"].PutValue(result.ToString());
                
                Console.WriteLine("Method executed successfully with parameters (Double, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDateTimeFromDouble method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MethodGetDateTimeFromDoubleDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


