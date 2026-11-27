---
title: "PivotShowValuesSetting.BaseItemPositionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotShowValuesSetting egenskap. Representerar typen av bas-pivotelementet i basfältet när ShowDataAs-beräkningen används. Eftersom PivotItemPosition.Custom endast är för läsning, om du behöver sätta PivotItemPosition.Custom, vänligen sätt attributet PivotField.BaseItemIndex."
type: docs
url: /sv/net/aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/
---
## PivotShowValuesSetting.BaseItemPositionType property

Representerar typen av bas-pivotelementet i basfältet när ShowDataAs-beräkningen används. Eftersom PivotItemPosition.Custom endast är för läsning, om du behöver sätta PivotItemPosition.Custom, vänligen sätt attributet PivotField.BaseItemIndex.

```csharp
[Obsolete("Use PivotShowValuesSetting.BaseItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotItemPositionType BaseItemPositionType { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotShowValuesSetting.BaseItem-egenskapen. Denna metod kommer att tas bort 12 månader senare, från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotShowValuesSettingPropertyBaseItemPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotField dataField = pivotTable.DataFields[0];
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0;
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1;

            pivotTable.RefreshData();
            pivotTable.CalculateData();

            workbook.Save("PivotShowValuesSettingExample.xlsx");
        }
    }
}
```

### Se även

* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


