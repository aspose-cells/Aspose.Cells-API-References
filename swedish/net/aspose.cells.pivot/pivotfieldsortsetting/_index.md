---
title: "Klass PivotFieldSortSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFieldSortSetting klass. Representerar inställningen för sortering av pivottabellsfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

Representerar inställningen för sortering av pivottfält.

```csharp
public class PivotFieldSortSetting
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | Sorterar efter värdena i vilken rad eller kolumn. |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; set; } | (**Föråldrad.**) Representerar indexet för fältet som sorteras efter. -1 betyder att PivotField sorteras efter etiketter, andra betyder sortering efter datafältet. |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; set; } | Indikerar om en enkel datasorteringsoperation kommer att tillämpas. |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | Indikerar om fältet ska sorteras efter sig självt eller datafältet. |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | Pivotlinjetypen som sorteras efter. |
| [SortBy](../../aspose.cells.pivot/pivotfieldsortsetting/sortby/) { get; set; } | Representerar indexet för fältet som sorteras efter. Ett värde på -1 indikerar sortering efter pivotelementets egna värden. När värdet är större än eller lika med noll representerar det indexet för datafältet i dataområdet. |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; set; } | Representerar [`SortOrder`](../../aspose.cells/sortorder/). |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hämta sorteringsinställning för pivottabellens fält
            // Obs: Detta förutsätter att pivottabellen har sorteringsinställningar som vi kan komma åt
            // Eftersom vi inte kan skapa en ny PivotFieldSortSetting direkt
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // Visningsegenskaper (endast läsning)
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // Tillämpa sortering på pivottabellen (faktisk sortering skulle göras via pivottabellmetoder)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara resultatet
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


