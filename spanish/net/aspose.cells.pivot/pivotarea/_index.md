---
title: "Clase PivotArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotArea. Presenta el área seleccionada de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/
---
## PivotArea class

Presenta el área seleccionada de la tabla dinámica.

```csharp
public class PivotArea
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | Presenta el área seleccionada de la PivotTable. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | Obtiene y establece la región de la PivotTable a la que se aplica esta regla. |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | Obtiene todos los filtros para esta PivotArea. |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | Indica si el total general de la columna está incluido. |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | Indica si la regla se refiere a un área que está en modo de esquema. |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | Indica si se incluye el total general de la fila. |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | Indica si solo se seleccionan los valores de datos (en el área de datos de la vista) para una selección de elemento y no se incluyen las etiquetas del elemento. |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | Indica si solo se seleccionan las etiquetas de datos para una selección de elemento. |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | Obtiene y establece el tipo de regla de selección. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | Obtiene las áreas de celdas de esta área de tabla dinámica. |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | Selecciona el área con filtros. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | Selecciona un campo en la región como un área. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | Selecciona un campo en la región como un área. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaDemo
    {
        public static void PivotAreaExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Agregar una tabla dinámica a la hoja de cálculo
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Crear una instancia de PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);

            // Establecer propiedades del PivotArea
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // Usar el método Select para seleccionar un área específica
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Guarda el libro de trabajo
            workbook.Save("PivotAreaExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


