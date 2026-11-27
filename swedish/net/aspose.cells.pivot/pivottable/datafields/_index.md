---
title: "PivotTable.DataFields"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar en PivotFieldCollection som representerar alla datafält i en PivotTable"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/datafields/
---
## PivotTable.DataFields property

Hämtar en [`PivotFieldCollection`](../../pivotfieldcollection/) som representerar alla datafält i en PivotTable.

```csharp
public PivotFieldCollection DataFields { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Lägg till en pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Åtkomst till datafält och demonstrera funktionalitet
            PivotFieldCollection dataFields = pivotTable.DataFields;
            if (dataFields.Count > 0)
            {
                PivotField dataField = dataFields[0];
                Console.WriteLine("Data Field Name: " + dataField.Name);
                Console.WriteLine("Data Field Function: " + dataField.Function);
            }

            // Spara arbetsboken
            workbook.Save("PivotTableDataFieldsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


