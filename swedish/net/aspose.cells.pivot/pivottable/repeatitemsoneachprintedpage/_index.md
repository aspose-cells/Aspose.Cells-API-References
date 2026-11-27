---
title: "PivotTable.RepeatItemsOnEachPrintedPage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om rubriker för pivotelement i radområdet upprepas på varje utskriven sida för pivotfält i tabellform"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/
---
## PivotTable.RepeatItemsOnEachPrintedPage property

Anger om rubriker för pivotelement i radområdet upprepas på varje utskriven sida för pivofält i tabellformat.

```csharp
public bool RepeatItemsOnEachPrintedPage { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRepeatItemsOnEachPrintedPageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("North");
            worksheet.Cells["A4"].PutValue("South");
            worksheet.Cells["A5"].PutValue("South");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Apples");
            worksheet.Cells["B3"].PutValue("Oranges");
            worksheet.Cells["B4"].PutValue("Apples");
            worksheet.Cells["B5"].PutValue("Oranges");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["C5"].PutValue(2500);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ställ in sidinställning för utskrift
            worksheet.PageSetup.PrintTitleRows = "$1:$1";
            worksheet.PageSetup.PrintArea = "A1:G20";
            worksheet.PageSetup.FitToPagesTall = 0;
            worksheet.PageSetup.FitToPagesWide = 1;

            // Visa aktuellt RepeatItemsOnEachPrintedPage-värde
            Console.WriteLine("Current RepeatItemsOnEachPrintedPage value: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // Aktivera upprepning av objekt på varje utskriven sida
            pivotTable.RepeatItemsOnEachPrintedPage = true;
            Console.WriteLine("RepeatItemsOnEachPrintedPage set to: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // Beräkna data för att fylla pivottabellen
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableRepeatItemsOnEachPrintedPageDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


