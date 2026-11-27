---
title: "Enum PivotFieldDataDisplayFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFieldDataDisplayFormat enum. Representerar data visningsformat i PivotTable-datafältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfielddatadisplayformat/
---
## PivotFieldDataDisplayFormat enumeration

Representerar data­visningsformat i PivotTable‑datafältet.

```csharp
public enum PivotFieldDataDisplayFormat
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Normal | `0` | Representerar normalt visningsformat. |
| DifferenceFrom | `1` | Representerar skillnad från visningsformat. |
| PercentageOf | `2` | Representerar procent av visningsformat. |
| PercentageDifferenceFrom | `3` | Representerar procentuell skillnad från visningsformat. |
| RunningTotalIn | `4` | Representerar löpande total i visningsformat. |
| PercentageOfRow | `5` | Representerar procent av radens visningsformat. |
| PercentageOfColumn | `6` | Representerar procent av kolumnens visningsformat. |
| PercentageOfTotal | `7` | Representerar procent av totalens visningsformat. |
| Index | `8` | Representerar indexvisningsformat. |
| PercentageOfParentRowTotal | `9` | Representerar procent av förälderradens totala visningsformat. |
| PercentageOfParentColumnTotal | `10` | Representerar procent av föräldrakolumnens totala visningsformat. |
| PercentageOfParentTotal | `11` | Representerar procent av föräldratotalens visningsformat. |
| PercentageOfRunningTotalIn | `12` | Representerar procent av löpande total i visningsformat. |
| RankSmallestToLargest | `13` | Representerar minsta till största visningsformat. |
| RankLargestToSmallest | `14` | Representerar största till minsta visningsformat. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDataDisplayFormatDemo
    {
        public static void PivotFieldDataDisplayFormatExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Lägg till lite exempeldata
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Lägg till en pivottabell
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Ställ in pivottabellens stil
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Ändra attribut för PivotField
            PivotField dataField = pivot.DataFields[0];
            dataField.DisplayName = "custom display name";

            // Ställ in DataDisplayFormat
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;

            // Uppdatera och beräkna data
            pivot.RefreshData();
            pivot.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotFieldDataDisplayFormatExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


