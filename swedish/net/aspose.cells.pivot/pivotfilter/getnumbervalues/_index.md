---
title: "PivotFilter.GetNumberValues"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter-metod. Hämtar värdena för numeriskt filter"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/getnumbervalues/
---
## PivotFilter.GetNumberValues method

Hämtar värden för talfiltret.

```csharp
public double[] GetNumberValues()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetNumberValuesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 5;
            sheet.Cells["B3"].Value = 3;
            sheet.Cells["B4"].Value = 2;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Tillämpa värdefilter
            pivotTable.RowFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 4, 0);
            
            // Hämta och visa filtervärden
            PivotFilter filter = pivotTable.RowFields[0].GetFilters()[0];
            double[] numberValues = filter.GetNumberValues();
            
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Number Values: " + string.Join(", ", numberValues));
        }
    }
}
```

### Se även

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


