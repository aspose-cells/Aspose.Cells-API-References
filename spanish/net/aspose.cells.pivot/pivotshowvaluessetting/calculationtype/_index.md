---
title: "PivotShowValuesSetting.CalculationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotShowValuesSetting propiedad. Representa cómo mostrar los valores de un campo de datos en el informe de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotshowvaluessetting/calculationtype/
---
## PivotShowValuesSetting.CalculationType property

Representa cómo mostrar los valores de un campo de datos en el informe de tabla dinámica.

```csharp
[Obsolete("Use PivotShowValuesSetting.ShowValuesAs property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldDataDisplayFormat CalculationType { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad PivotShowValuesSetting.ShowValuesAs. Este método será eliminado 12 meses después a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
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

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Agregar campo de datos y establecer el tipo de cálculo
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.RankLargestToSmallest;

            // Calcular datos y guardar
            pivotTable.CalculateData();
            workbook.Save("PivotShowValuesSettingPropertyCalculationTypeDemo_out.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


