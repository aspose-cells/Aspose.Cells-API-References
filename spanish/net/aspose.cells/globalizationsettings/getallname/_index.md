---
title: "GlobalizationSettings.GetAllName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de la etiqueta All en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getallname/
---
## GlobalizationSettings.GetAllName method

Obtiene el nombre de la etiqueta "(All)" en la tabla dinámica.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfAll() method instead.")]
public virtual string GetAllName()
```

### Valor de retorno

El nombre de la etiqueta "(All)"

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método GlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetAllNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con configuraciones de globalización personalizadas
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Acceder a la instancia de configuraciones personalizadas
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            try
            {
                // Llame al método GetAllName y muestre el resultado
                string allName = settings.GetAllName();
                Console.WriteLine($"Custom (All) label: {allName}");

                // Cree una tabla dinámica de ejemplo para demostrar el efecto de la localización
                Worksheet worksheet = workbook.Worksheets[0];
                CreateSampleData(worksheet);
                CreatePivotTable(worksheet);

                Console.WriteLine("Demo executed successfully. Check output file's pivot table labels.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("MethodGetAllNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Crear datos de muestra para tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Cars";
            worksheet.Cells["A4"].Value = "Bikes";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["B4"].Value = 1500;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Cree una tabla dinámica usando datos de ejemplo
            int pivotIndex = worksheet.PivotTables.Add(
                "PivotTable",
                "A1:B4",
                "E3"
            );
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Configure la estructura de la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields[0]); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields[1]); // Sales

            // Actualice la tabla para aplicar la configuración de localización
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetAllName()
        {
            // La implementación personalizada devuelve la etiqueta "All" localizada
            return "[Custom All Selection]";
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


