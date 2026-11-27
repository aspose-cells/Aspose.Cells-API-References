---
title: "PivotFieldSortSetting.IsSimpleSort"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldSortSetting-egenskap. Anger om en enkel datasortering kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldsortsetting/issimplesort/
---
## PivotFieldSortSetting.IsSimpleSort property

Indikerar om en enkel datasorteringsoperation kommer att tillämpas.

```csharp
public bool IsSimpleSort { get; set; }
```

### Anmärkningar

Standardvärdet är sant.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSimpleSortDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 150;
            worksheet.Cells["B6"].Value = 250;

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hämta pivottfältet
            PivotField pivotField = pivotTable.RowFields[0];

            // Hämta sorteringsinställning (skrivskyddad egenskap)
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Visa aktuellt värde för IsSimpleSort
            Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);

            // Obs: IsSimpleSort är skrivskyddad, så vi kan inte sätta den direkt
            // För att demonstrera sortering skapar vi en ny pivottabell med annan sortering

            // Skapa en annan pivottabell med anpassad sortering
            pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
            PivotTable pivotTable2 = pivotTables[pivotIndex];
            pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Sortera pivottfältet med tillgänglig metod
            PivotField pivotField2 = pivotTable2.RowFields[0];
            pivotField2.SortBy(SortOrder.Ascending, -1);

            // Spara arbetsboken
            workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


