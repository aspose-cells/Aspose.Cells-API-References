---
title: "GlobalizationSettings.GetProtectionNameOfPivotTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de protección en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getprotectionnameofpivottable/
---
## GlobalizationSettings.GetProtectionNameOfPivotTable method

Obtiene el nombre de protección en la tabla dinámica.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetProtectionNameOfPivotTable()
```

### Valor de retorno

El nombre de protección de la tabla dinámica

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetTextOfProtectedName(string). Esta propiedad será eliminada 12 meses después, a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear configuraciones de globalización estándar
            GlobalizationSettings standardSettings = new GlobalizationSettings();
            
            // Cree configuraciones de globalización personalizadas
            GlobalizationSettings customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Obtener el nombre de protección predeterminado
                string defaultName = standardSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Default protection name: {defaultName}");

                // Obtener el nombre de protección personalizado
                string customName = customSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Custom protection name: {customName}");

                // Crear tabla dinámica para demostrar la aplicación de configuraciones
                worksheet.Cells["A1"].Value = "Data";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;
                int pivotIndex = worksheet.PivotTables.Add("A1", "A1:A4", "PivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // La protección normalmente se aplicaría aquí usando el nombre obtenido
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetProtectionNameOfPivotTable: {ex.Message}");
            }
            
            workbook.Save("GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public new string GetProtectionNameOfPivotTable()
        {
            return "CustomPivotProtection";
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


