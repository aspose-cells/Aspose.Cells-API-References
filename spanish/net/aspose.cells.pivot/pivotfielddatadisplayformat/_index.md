---
title: "Enumeración PivotFieldDataDisplayFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Pivot.PivotFieldDataDisplayFormat. Representa el formato de visualización de datos en el campo de datos de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotfielddatadisplayformat/
---
## PivotFieldDataDisplayFormat enumeration

Representa el formato de visualización de datos en el campo de datos de la tabla dinámica.

```csharp
public enum PivotFieldDataDisplayFormat
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Normal | `0` | Representa el formato de visualización normal. |
| DifferenceFrom | `1` | Representa la diferencia del formato de visualización. |
| PercentageOf | `2` | Representa el porcentaje del formato de visualización. |
| PercentageDifferenceFrom | `3` | Representa la diferencia porcentual del formato de visualización. |
| RunningTotalIn | `4` | Representa el total acumulado en el formato de visualización. |
| PercentageOfRow | `5` | Representa el porcentaje del formato de visualización de fila. |
| PercentageOfColumn | `6` | Representa el porcentaje del formato de visualización de columna. |
| PercentageOfTotal | `7` | Representa el porcentaje del formato de visualización total. |
| Index | `8` | Representa el formato de visualización de índice. |
| PercentageOfParentRowTotal | `9` | Representa el porcentaje del formato de visualización del total de fila padre. |
| PercentageOfParentColumnTotal | `10` | Representa el porcentaje del formato de visualización del total de columna padre. |
| PercentageOfParentTotal | `11` | Representa el porcentaje del formato de visualización del total padre. |
| PercentageOfRunningTotalIn | `12` | Representa el porcentaje del total acumulado en el formato de visualización. |
| RankSmallestToLargest | `13` | Representa el formato de visualización de menor a mayor. |
| RankLargestToSmallest | `14` | Representa el formato de visualización de mayor a menor. |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Agregar algunos datos de ejemplo
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

            // Agregar una tabla dinámica
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Establecer el estilo de tabla dinámica
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Cambiar los atributos del PivotField
            PivotField dataField = pivot.DataFields[0];
            dataField.DisplayName = "custom display name";

            // Establecer DataDisplayFormat
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;

            // Actualizar y calcular datos
            pivot.RefreshData();
            pivot.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldDataDisplayFormatExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


