---
title: "PivotTable.ShowEmptyCol"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om tomma kolumner ska inkluderas i tabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showemptycol/
---
## PivotTable.ShowEmptyCol property

Anger om tomma kolumner ska inkluderas i tabellen

```csharp
public bool ShowEmptyCol { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyColDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa det aktuella värdet för ShowEmptyCol
            Console.WriteLine("Current ShowEmptyCol value: " + pivotTable.ShowEmptyCol);

            // Ställ in ShowEmptyCol till false (dölj tomma kolumner)
            pivotTable.ShowEmptyCol = false;
            Console.WriteLine("ShowEmptyCol set to false - empty columns will be hidden");

            // Beräkna pivottabellsdata
            pivotTable.CalculateData();

            // Spara arbetsboken med dolda tomma kolumner
            workbook.Save("PivotTableHideEmptyCols.xlsx");

            // Ställ in ShowEmptyCol tillbaka till true (visa tomma kolumner)
            pivotTable.ShowEmptyCol = true;
            Console.WriteLine("ShowEmptyCol set to true - empty columns will be shown");

            // Beräkna pivottabellens data igen
            pivotTable.CalculateData();

            // Spara arbetsboken med synliga tomma kolumner
            workbook.Save("PivotTableShowEmptyCols.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


