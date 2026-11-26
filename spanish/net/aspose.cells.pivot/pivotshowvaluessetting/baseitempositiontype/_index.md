---
title: "PivotShowValuesSetting.BaseItemPositionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotShowValuesSetting. Representa el tipo del elemento pivote base en el campo base cuando se está utilizando el cálculo ShowDataAs. Debido a que PivotItemPosition.Custom es solo de lectura, si necesita establecer PivotItemPosition.Custom, establezca el atributo PivotField.BaseItemIndex."
type: docs
url: /es/net/aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/
---
## PivotShowValuesSetting.BaseItemPositionType property

Representa el tipo del elemento pivote base en el campo base cuando se está utilizando el cálculo ShowDataAs. Debido a que PivotItemPosition.Custom es solo de lectura, si necesita establecer PivotItemPosition.Custom, establezca el atributo PivotField.BaseItemIndex.

```csharp
[Obsolete("Use PivotShowValuesSetting.BaseItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotItemPositionType BaseItemPositionType { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotShowValuesSetting.BaseItem. Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

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

### Ver también

* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


