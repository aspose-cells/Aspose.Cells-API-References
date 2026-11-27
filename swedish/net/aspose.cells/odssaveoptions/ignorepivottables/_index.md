---
title: "OdsSaveOptions.IgnorePivotTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsSaveOptions‑egenskap. Anger om pivottabeller ska sparas"
type: docs
url: /sv/net/aspose.cells/odssaveoptions/ignorepivottables/
---
## OdsSaveOptions.IgnorePivotTables property

Anger om pivottabeller ska sparas.

```csharp
public bool IgnorePivotTables { get; set; }
```

### Anmärkningar

Pivottabellfunktionen i OpenOffice har färre inställningar jämfört med Excel, så deras pivottabellsresultat har många skillnader. Ibland är det bättre att ignorera dessa pivottabeller när .ods‑filen sparas.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Skapa en pivottabell
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa OdsSaveOptions‑instans
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Visa aktuellt värde för IgnorePivotTables
            Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);

            // Ställ in att ignorera pivottabeller vid sparande
            saveOptions.IgnorePivotTables = true;

            // Spara med pivottabeller ignorerade
            workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);

            // Ställ in att inkludera pivottabeller vid sparande
            saveOptions.IgnorePivotTables = false;

            // Spara med pivottabeller inkluderade
            workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
        }
    }
}
```

### Se även

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


