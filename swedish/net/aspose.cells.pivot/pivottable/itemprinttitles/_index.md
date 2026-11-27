---
title: "PivotTable.ItemPrintTitles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om PivotItem-namn ska upprepas högst upp på varje utskriven sida"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/itemprinttitles/
---
## PivotTable.ItemPrintTitles property

Anger om PivotItem-namn ska upprepas högst upp på varje utskriven sida.

```csharp
[Obsolete("Use PivotTable.RepeatItemsOnEachPrintedPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ItemPrintTitles { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotTable.RepeatItemsOnEachPrintedPage. Denna metod kommer att tas bort 12 månader senare från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyItemPrintTitlesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);
            worksheet.Cells["A5"].PutValue("Product D");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(4000);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa det aktuella värdet av ItemPrintTitles
            Console.WriteLine("Current ItemPrintTitles value: " + pivotTable.ItemPrintTitles);

            // Ställ in ItemPrintTitles till true (detta är föråldrat, men visas för demonstration)
            pivotTable.ItemPrintTitles = true;

            // Alternativt, använd den icke-föråldrade egenskapen
            pivotTable.RepeatItemsOnEachPrintedPage = true;

            // Uppdatera och beräkna pivottabellen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableItemPrintTitlesDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


