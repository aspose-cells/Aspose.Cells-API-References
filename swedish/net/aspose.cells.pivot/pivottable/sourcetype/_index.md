---
title: "PivotTable.SourceType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑egenskap. Hämtar datakälltyp för pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/sourcetype/
---
## PivotTable.SourceType property

Hämtar datakälltyp för pivottabellen.

```csharp
public PivotTableSourceType SourceType { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertySourceTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Product A";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Product B";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Product C";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa det aktuella SourceType‑värdet
            Console.WriteLine("Current PivotTable SourceType: " + pivotTable.SourceType);

            // Beräkna data för att visa pivottabellen
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableSourceTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotTableSourceType](../../pivottablesourcetype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


