---
title: "PivotFieldSortSetting.IsSortByLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldSortSetting-egenskap. Anger om fältet ska sorteras efter sig själv eller efter datafältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/
---
## PivotFieldSortSetting.IsSortByLabels property

Indikerar om fältet ska sorteras efter sig självt eller datafältet.

```csharp
public bool IsSortByLabels { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSortByLabelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Hämta pivottfältets sorteringsinställning
            PivotField pivotField = pivotTable.RowFields[0];
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Visa aktuellt värde för IsSortByLabels
            Console.WriteLine("Current IsSortByLabels value: " + sortSetting.IsSortByLabels);

            // Obs: IsSortByLabels är skrivskyddad, så vi kan inte sätta den direkt
            // Istället demonstrerar vi dess betydelse genom att undersöka sorteringsinställningarna

            // Visa relaterade sorteringsegenskaper
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);

            // Spara arbetsboken
            workbook.Save("PivotFieldSortSettingPropertyIsSortByLabelsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


