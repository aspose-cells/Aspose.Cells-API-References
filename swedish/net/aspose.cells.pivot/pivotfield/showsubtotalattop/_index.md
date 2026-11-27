---
title: "PivotField.ShowSubtotalAtTop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger om delsummer ska visas högst upp eller längst ner på objekten"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/showsubtotalattop/
---
## PivotField.ShowSubtotalAtTop property

Anger om delsummer ska visas högst upp eller längst ner på objekten.

```csharp
public bool ShowSubtotalAtTop { get; set; }
```

### Anmärkningar

Fungerar endast för pivottfälten i radregionen när ShowInOutlineForm är sant.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowSubtotalAtTopDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["B3"].Value = 1500;
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["B4"].Value = 2000;
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B5"].Value = 2500;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Lägg till radfält och konfigurera delsummeringsposition
            PivotField rowField = pivotTable.RowFields[pivotTable.AddFieldToArea(PivotFieldType.Row, "Product")];
            rowField.ShowSubtotalAtTop = true; // Demonstrate the property
            rowField.IsAutoSubtotals = true;

            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Spara arbetsboken
            workbook.Save("PivotFieldShowSubtotalAtTopDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


