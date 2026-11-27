---
title: "PivotShowValuesSetting.CalculationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotShowValuesSetting‑egenskapen. Representerar hur värden för ett datafält visas i pivotrappporten"
type: docs
url: /sv/net/aspose.cells.pivot/pivotshowvaluessetting/calculationtype/
---
## PivotShowValuesSetting.CalculationType property

Representerar hur värden för ett datafält visas i pivotrappporten.

```csharp
[Obsolete("Use PivotShowValuesSetting.ShowValuesAs property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldDataDisplayFormat CalculationType { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Använd istället PivotShowValuesSetting.ShowValuesAs‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotShowValuesSettingPropertyCalculationTypeDemo
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
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Lägg till datafält och ställ in beräkningstyp
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.RankLargestToSmallest;

            // Beräkna data och spara
            pivotTable.CalculateData();
            workbook.Save("PivotShowValuesSettingPropertyCalculationTypeDemo_out.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


