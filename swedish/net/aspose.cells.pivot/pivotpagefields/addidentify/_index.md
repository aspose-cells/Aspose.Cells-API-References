---
title: "PivotPageFields.AddIdentify"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotPageFields‑metod. Anger vilken objektetikett i varje sidfält som ska användas för att identifiera dataområdet. pageItemIndex.Length måste vara lika med PageFieldCount, så lägg till sidfältet först."
type: docs
url: /sv/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Anger vilken objektetikett i varje sidfält som ska användas för att identifiera dataintervallet. pageItemIndex.Length måste vara lika med PageFieldCount, så lägg till sidfältet först.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rangeIndex | Int32 | Konsolideringsdataområdesindexet. |
| pageItemIndex | Int32[] | Sidobjektets index i varje sidfält. pageItemIndex[2] = 1 betyder att det andra objektet i det tredje fältet används för att identifiera detta område. pageItemIndex[1] = -1 betyder att inget objekt i det andra fältet används för att identifiera detta område och MS kommer automatiskt att skapa ett \"blank\" objekt i det andra fältet för att identifiera detta område. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");
            worksheet.Cells["B4"].PutValue("C");

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Instansiera PivotPageFields direkt istället för att komma åt via PivotTable
            PivotPageFields pageFields = new PivotPageFields();

            try
            {
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                Console.WriteLine("AddIdentify executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


