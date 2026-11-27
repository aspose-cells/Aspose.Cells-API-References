---
title: "Name.GetRefersTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-metod. Hämtar referensen för detta namn"
type: docs
url: /sv/net/aspose.cells/name/getrefersto/
---
## GetRefersTo(bool, bool) {#getrefersto}

Hämta referensen för detta Name.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om referensen behöver formateras som R1C1. |
| isLocal | Boolean | Om referensen behöver formateras enligt lokala inställningar. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Skapa ett namngivet område
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Anropa GetRefersTo med R1C1-format och lokal omfattning
                string refersToR1C1Local = namedRange.GetRefersTo(true, true);
                Console.WriteLine("R1C1 format with local scope: " + refersToR1C1Local);

                // Anropa GetRefersTo med A1-format och global omfattning
                string refersToA1Global = namedRange.GetRefersTo(false, false);
                Console.WriteLine("A1 format with global scope: " + refersToA1Global);

                // Visa detaljer för det namngivna området
                Console.WriteLine("Named range text: " + namedRange.Text);
                Console.WriteLine("Full text: " + namedRange.FullText);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("NameMethodGetRefersToDemo.xlsx");
        }
    }
}
```

### Se även

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRefersTo(bool, bool, int, int) {#getrefersto_1}

Hämta referensen för detta Name baserat på angiven cell.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om referensen behöver formateras som R1C1. |
| isLocal | Boolean | Om referensen behöver formateras enligt lokala inställningar. |
| row | Int32 | Radindex för cellen. |
| column | Int32 | Kolumnindex för cellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo
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
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Anropa GetRefersTo med specifika parametrar (isR1C1, isLocal, rad, kolumn)
                string refersTo = namedRange.GetRefersTo(false, false, 0, 0);
                
                Console.WriteLine("Named range refers to: " + refersTo);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");

                // Ändra det namngivna området baserat på resultatet
                if (!string.IsNullOrEmpty(refersTo))
                {
                    worksheet.Cells["B1"].PutValue("Named Range Refers To:");
                    worksheet.Cells["B2"].PutValue(refersTo);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


