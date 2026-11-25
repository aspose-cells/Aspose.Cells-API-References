---
title: "PivotShowValuesSetting.BaseItemPositionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotShowValuesSetting. Rappresenta il tipo dell'elemento pivot base nel campo base quando il calcolo ShowDataAs è in uso. Poiché PivotItemPosition.Custom è solo in lettura, se è necessario impostare PivotItemPosition.Custom, impostare l'attributo PivotField.BaseItemIndex."
type: docs
url: /it/net/aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/
---
## PivotShowValuesSetting.BaseItemPositionType property

Rappresenta il tipo dell'elemento pivot base nel campo base quando il calcolo ShowDataAs è in uso. Poiché PivotItemPosition.Custom è solo in lettura, se è necessario impostare PivotItemPosition.Custom, impostare l'attributo PivotField.BaseItemIndex.

```csharp
[Obsolete("Use PivotShowValuesSetting.BaseItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotItemPositionType BaseItemPositionType { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotShowValuesSetting.BaseItem. Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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

### Vedi anche

* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


