---
title: "Cell.GetFormatConditions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑metod. Hämtar formatvillkor som gäller för den här cellen"
type: docs
url: /sv/net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Hämtar formatvillkor som gäller för denna cell.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Returvärde

Returnerar [`FormatConditionCollection`](../../formatconditioncollection/) objekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormatConditionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta cellsamling
            Cells cells = worksheet.Cells;
            
            // Lägg till exempeldata
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            
            // Lägg till formatvillkor till cell A1
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            
            // Hämta formatvillkor för cell A1
            FormatConditionCollection[] conditions = cells["A1"].GetFormatConditions();
            
            // Skriv ut antalet formatvillkor
            Console.WriteLine("Number of format conditions: " + conditions.Length);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


