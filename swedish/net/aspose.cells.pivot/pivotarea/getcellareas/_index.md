---
title: "PivotArea.GetCellAreas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotArea-metod. Hämtar cellområden för detta pivotområde"
type: docs
url: /sv/net/aspose.cells.pivot/pivotarea/getcellareas/
---
## PivotArea.GetCellAreas method

Hämtar cellområden för detta pivområde.

```csharp
public CellArea[] GetCellAreas()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaMethodGetCellAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa minimal pivottabelldata
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";

            try
            {
                // Skapa pivottabell med grundläggande konfiguration
                int pivotIndex = worksheet.PivotTables.Add("A1:A3", "D1", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Initiera pivotområde med pivottabellinstansen
                PivotArea pivotArea = new PivotArea(pivotTable);

                // Konfigurera inställningar för pivotområde
                pivotArea.RuleType = PivotAreaType.Normal;
                pivotArea.AxisType = PivotFieldType.Data;
                pivotArea.IsRowGrandIncluded = true;

                // Kör målmetod
                CellArea[] cellAreas = pivotArea.GetCellAreas();

                Console.WriteLine($"GetCellAreas returned {cellAreas.Length} cell area(s)");
                foreach (CellArea area in cellAreas)
                {
                    Console.WriteLine($"CellArea: Columns {area.StartColumn}-{area.EndColumn}, Rows {area.StartRow}-{area.EndRow}");
                }

                workbook.Save("GetCellAreasDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetCellAreas: {ex.Message}");
            }
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


