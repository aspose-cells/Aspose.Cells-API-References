---
title: "PivotTable.TableRange1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Returnerar ett CellArea-objekt som representerar området som innehåller hela PivotTable-rapporten men som inte inkluderar sidfält. Endast läs"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/tablerange1/
---
## PivotTable.TableRange1 property

Returnerar ett CellArea‑objekt som representerar det område som innehåller hela PivotTable‑rapporten, men som inte inkluderar sidfält. Endast läsning.

```csharp
public CellArea TableRange1 { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange1Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad med exempeldata
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Skapa en pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            int pivotTableIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            
            // Lägg till fält i pivottabell
            int labelFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Konfigurera pivottabell
            pivotTable.ShowInTabularForm();
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demonstrera TableRange1-egenskapen
            Console.WriteLine("Pivot Table Range:");
            Console.WriteLine($"Start Row: {pivotTable.TableRange1.StartRow}");
            Console.WriteLine($"End Row: {pivotTable.TableRange1.EndRow}");
            Console.WriteLine($"Start Column: {pivotTable.TableRange1.StartColumn}");
            Console.WriteLine($"End Column: {pivotTable.TableRange1.EndColumn}");

            // Spara arbetsboken
            workbook.Save("PivotTablePropertyTableRange1Demo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


