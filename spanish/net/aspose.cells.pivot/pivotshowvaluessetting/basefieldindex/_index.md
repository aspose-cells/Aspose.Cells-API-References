---
title: "PivotShowValuesSetting.BaseFieldIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotShowValuesSetting propiedad. Representa el campo base para un cálculo ShowDataAs cuando el cálculo ShowDataAs está en uso"
type: docs
url: /es/net/aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/
---
## PivotShowValuesSetting.BaseFieldIndex property

Representa el campo base para un cálculo ShowDataAs cuando se utiliza el cálculo ShowDataAs.

```csharp
public int BaseFieldIndex { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
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
                // Crear tabla dinámica
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Agregar campos a la tabla dinámica
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Obtener el campo de datos y su configuración de mostrar valores
                PivotField dataField = pivotTable.DataFields[0];
                PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

                // Establecer el tipo de cálculo para demostrar el uso de BaseFieldIndex
                showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;

                // Establecer y obtener la propiedad BaseFieldIndex
                showValuesSetting.BaseFieldIndex = 0;
                Console.WriteLine("BaseFieldIndex value: " + showValuesSetting.BaseFieldIndex);

                // Actualizar y calcular la tabla dinámica
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Guarda el libro de trabajo
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

### Ver también

* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


