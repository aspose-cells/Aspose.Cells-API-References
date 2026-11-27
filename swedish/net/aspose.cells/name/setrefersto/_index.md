---
title: "Name.SetRefersTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-metod. Ange referensen för detta Name"
type: docs
url: /sv/net/aspose.cells/name/setrefersto/
---
## Name.SetRefersTo method

Ange referensen för detta Name.

```csharp
public void SetRefersTo(string refersTo, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| refersTo | String | Referensen. |
| isR1C1 | Boolean | Om referensen är i R1C1-format. |
| isLocal | Boolean | Om referensen är lokalanpassad. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodSetRefersToWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Skapa ett namngivet område
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];

            try
            {
                // Anropa SetRefersTo med parametrarna (String, Boolean, Boolean)
                namedRange.SetRefersTo("=Sheet1!$A$1:$A$3", false, false);

                // Visa resultatet
                Console.WriteLine($"Named range 'MyNamedRange' now refers to: {namedRange.RefersTo}");

                // Verifiera genom att använda det namngivna området i en formel
                worksheet.Cells["B1"].Formula = "=SUM(MyNamedRange)";
                workbook.CalculateFormula();

                Console.WriteLine($"Result of SUM(MyNamedRange): {worksheet.Cells["B1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRefersTo method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("NameMethodSetRefersToWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


