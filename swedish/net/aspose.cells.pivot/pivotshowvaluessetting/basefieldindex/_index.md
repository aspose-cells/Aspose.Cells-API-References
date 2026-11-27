---
title: "PivotShowValuesSetting.BaseFieldIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotShowValuesSetting‑egenskapen. Representerar basfältet för en ShowDataAs‑beräkning när ShowDataAs‑beräkningen används"
type: docs
url: /sv/net/aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/
---
## PivotShowValuesSetting.BaseFieldIndex property

Representerar basfältet för en ShowDataAs-beräkning när ShowDataAs-beräkningen används.

```csharp
public int BaseFieldIndex { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingPropertyBaseFieldIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            try
            {
                // Skapa pivottabell
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Lägg till fält i pivottabell
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Hämta datafältet och dess show values‑inställning
                PivotField dataField = pivotTable.DataFields[0];
                PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

                // Ställ in beräkningstyp för att demonstrera användning av BaseFieldIndex
                showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;

                // Ställ in och hämta BaseFieldIndex‑egenskapen
                showValuesSetting.BaseFieldIndex = 0;
                Console.WriteLine("BaseFieldIndex value: " + showValuesSetting.BaseFieldIndex);

                // Uppdatera och beräkna pivottabell
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Spara arbetsboken
                workbook.Save("BaseFieldIndexDemo.xlsx");
                Console.WriteLine("BaseFieldIndex has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


