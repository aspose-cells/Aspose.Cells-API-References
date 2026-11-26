---
title: "Clase PivotShowValuesSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Pivot.PivotShowValuesSetting class. Representa la configuración sobre cómo mostrar los valores cuando se utiliza el cálculo ShowDataAs."
type: docs
url: /es/net/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class

Representa la configuración sobre cómo mostrar los valores cuando se utiliza el cálculo ShowDataAs.

```csharp
public class PivotShowValuesSetting
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | Representa el campo base para un cálculo ShowDataAs cuando se utiliza el cálculo ShowDataAs. |
| [BaseFieldName](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldname/) { get; } | Obtiene el título del campo base de la tabla dinámica. |
| [BaseItemCaption](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemcaption/) { get; } | Obtiene el título del elemento de tabla dinámica en el campo base. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | Representa el índice personalizado del elemento de tabla dinámica en el campo base cuando se utiliza el cálculo ShowDataAs. |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | (**Obsolete.**) Representa el tipo del elemento base de la tabla dinámica en el campo base cuando se utiliza el cálculo ShowDataAs. Debido a que PivotItemPosition.Custom es solo de lectura, si necesita establecer PivotItemPosition.Custom, por favor establezca el atributo PivotField.BaseItemIndex. |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | (**Obsolete.**) Representa cómo mostrar los valores de un campo de datos en el informe de tabla dinámica. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotshowvaluessetting/showvaluesas/) { get; set; } | Obtiene y establece cómo mostrar los valores de un campo de datos en el informe de tabla dinámica. |

## Campos

| Nombre | Descripción |
| --- | --- |
| const [NextPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/nextpivotitem/) | Índice de elemento base especial: usar el elemento de tabla dinámica siguiente. Válido para los cálculos "Show Values As"; efectivo en Excel 2010 y versiones posteriores. |
| const [PreviousPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/previouspivotitem/) | Índice de elemento base especial: usar el elemento de tabla dinámica anterior. Válido para los cálculos "Show Values As"; efectivo en Excel 2010 y versiones posteriores. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingDemo
    {
        public static void PivotShowValuesSettingExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // Agregar una tabla dinámica a la hoja de cálculo
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Acceder al campo de datos
            PivotField dataField = pivotTable.DataFields[0];

            // Acceder a la propiedad ShowValuesSetting
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // Establecer propiedades de PivotShowValuesSetting
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // Actualizar y calcular los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


