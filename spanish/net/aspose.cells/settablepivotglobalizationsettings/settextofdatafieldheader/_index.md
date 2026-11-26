---
title: "SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Establece el texto del encabezado del campo del área de valores en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader method

Establece el texto del encabezado del campo del área de valores en la tabla dinámica.

```csharp
public void SetTextOfDataFieldHeader(string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto del nombre del encabezado del campo de datos |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfDataFieldHeaderWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // Crear una instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Establecer texto personalizado para el encabezado del campo de datos
                settings.SetTextOfDataFieldHeader("Custom Data Header");

                // Verificar el cambio obteniendo el texto actual
                string currentHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Data field header text: {currentHeaderText}");

                // Guarda el libro de trabajo para demostrar una ejecución exitosa
                workbook.Save("SetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("SetTextOfDataFieldHeader method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


