---
title: "PivotFieldCollection.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldCollection-egenskap. Hämtar PivotFields-typen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldcollection/type/
---
## PivotFieldCollection.Type property

Hämtar typen för PivotFields.

```csharp
public PivotFieldType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Visa typen av pivotfältssamlingen
            Console.WriteLine("PivotFieldCollection Type: " + rowFields.Type);

            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotFieldCollection dataFields = pivotTable.DataFields;

            // Visa typen av datfältssamlingen
            Console.WriteLine("DataFields Type: " + dataFields.Type);

            // Beräkna data och uppdatera pivottabellen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara resultatet
            workbook.Save("PivotFieldCollectionTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


