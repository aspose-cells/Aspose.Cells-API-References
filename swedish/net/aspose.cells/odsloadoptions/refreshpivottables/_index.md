---
title: "OdsLoadOptions.RefreshPivotTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsLoadOptions egenskap. Anger om pivottabeller ska uppdateras vid inläsning av fil"
type: docs
url: /sv/net/aspose.cells/odsloadoptions/refreshpivottables/
---
## OdsLoadOptions.RefreshPivotTables property

Anger om pivottabeller ska uppdateras vid inläsning av filen.

```csharp
public bool RefreshPivotTables { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Skapa ett exempel på arbetsbok med pivottabell
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["C1"].PutValue("Price");
            sheet.Cells["C2"].PutValue(2.5);
            sheet.Cells["C3"].PutValue(3.0);
            sheet.Cells["C4"].PutValue(1.5);

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");

            // Spara som ODS
            string odsPath = "output.ods";
            wb.Save(odsPath, SaveFormat.Ods);

            // Läs in med RefreshPivotTables aktiverat
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.RefreshPivotTables = true;
            Workbook wb2 = new Workbook(odsPath, loadOptions);

            // Verifiera att pivottabellen uppdaterades
            Console.WriteLine("Pivot table count: " + wb2.Worksheets[0].PivotTables.Count);
        }
    }
}
```

### Se även

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


