---
title: "GlobalizationSettings.GetMultipleItemsName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de la etiqueta Multiple Items en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getmultipleitemsname/
---
## GlobalizationSettings.GetMultipleItemsName method

Obtiene el nombre de la etiqueta "(Multiple Items)" en la tabla dinámica.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfMultipleItems() method instead.")]
public virtual string GetMultipleItemsName()
```

### Valor de retorno

El nombre de la etiqueta "(Multiple Items)"

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetMultipleItemsNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("D1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Configurar PivotField para mostrar múltiples elementos
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.HideItem(0, false); // Select "A"
            rowField.HideItem(1, false); // Select "B"

            // Inicializar configuraciones de globalización
            GlobalizationSettings gSettings = workbook.Settings.GlobalizationSettings ?? new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings = gSettings;

            try
            {
                // Llamar a GetMultipleItemsName y mostrar el resultado
                string multipleItemsName = gSettings.GetMultipleItemsName();
                Console.WriteLine($"Multiple Items Name: {multipleItemsName}");

                // Actualizar la tabla dinámica para aplicar la configuración
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetMultipleItemsName: {ex.Message}");
            }

            // Guardar el libro de trabajo para mostrar la tabla dinámica con la etiqueta de múltiples elementos
            workbook.Save("GlobalizationSettingsMethodGetMultipleItemsNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


