---
title: "SettableChartGlobalizationSettings.SetAxisUnitName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Establece el Nombre de la Unidad del Eje"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/setaxisunitname/
---
## SettableChartGlobalizationSettings.SetAxisUnitName method

Establece el nombre de la unidad del eje

```csharp
public void SetAxisUnitName(DisplayUnitType type, string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | DisplayUnitType | El tipo de unidad para mostrar etiquetas del eje. |
| name | String | nombre dependiente local |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetAxisUnitNameWithDisplayUnitTypeStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos mínimos para contexto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea una instancia de SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Establezca nombres de unidad de eje personalizados para diferentes tipos de DisplayUnitType
                settings.SetAxisUnitName(DisplayUnitType.Thousands, "K");
                settings.SetAxisUnitName(DisplayUnitType.Millions, "M");
                settings.SetAxisUnitName(DisplayUnitType.Percentage, "Pct");

                // Verifique la configuración recuperando los valores
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // Muestra los resultados
                Console.WriteLine($"Thousands unit name set to: {thousandsUnit}");
                Console.WriteLine($"Millions unit name set to: {millionsUnit}");
                Console.WriteLine($"Percentage unit name set to: {percentageUnit}");

                // Guarda el libro de trabajo
                workbook.Save("SetAxisUnitNameDemo.xlsx");
                Console.WriteLine("SetAxisUnitName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisUnitName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


