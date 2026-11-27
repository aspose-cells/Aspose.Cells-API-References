---
title: "FormatConditionCollection.AddArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatConditionCollection metod. Lägger till ett villkorligt formaterat cellområde"
type: docs
url: /sv/net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

Lägger till ett villkorligt formaterat cellområde.

```csharp
public int AddArea(CellArea cellArea)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | CellArea | Villkorsformaterat cellområde. |

### Returvärde

Index för villkorligt formaterat cellområde.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue(row * col);
                }
            }

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection formatCollection = worksheet.ConditionalFormattings[index];
            
            // Skapa formatvillkor
            formatCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Skapa cellområden och lägg till dem i formatkollektionen
            CellArea area1 = CellArea.CreateCellArea(0, 0, 4, 4);
            CellArea area2 = CellArea.CreateCellArea(5, 5, 9, 9);
            
            formatCollection.AddArea(area1);
            formatCollection.AddArea(area2);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


