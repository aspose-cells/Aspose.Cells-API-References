---
title: "UnionRange.PutValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange-metod. Lägger in ett värde i området; om lämpligt konverteras värdet till en annan datatyp och cellernas talformat återställs"
type: docs
url: /sv/net/aspose.cells/unionrange/putvalue/
---
## UnionRange.PutValue method

Sätter ett värde i området, om lämpligt konverteras värdet till en annan datatyp och cellens talformat återställs.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | String | Ange värde |
| isConverted | Boolean | True: konverterad till annan datatyp om lämpligt. |
| setStyle | Boolean | True: sätt talformatet till cellens stil vid konvertering till annan datatyp |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett UnionRange som täcker cellerna A1 till B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            
            try
            {
                // Anropa PutValue med parametrarna: (String, Boolean, Boolean)
                unionRange.PutValue("Sample Value", true, true);
                
                Console.WriteLine("PutValue method executed successfully with parameters (String, Boolean, Boolean)");
                
                // Visa områdesinformationen för att visa effekten
                Console.WriteLine($"Range address: {unionRange.RefersTo}");
                Console.WriteLine($"Value set in range: {unionRange.Value}");
                
                // Applicera formatering för att göra effekten synlig
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.HorizontalAlignment = TextAlignmentType.Center;
                unionRange.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PutValue method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("UnionRangeMethodPutValueWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


