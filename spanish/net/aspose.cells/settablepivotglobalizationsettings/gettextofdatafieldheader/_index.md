---
title: "SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Obtiene el texto del encabezado del campo del área de valores en la PivotTable"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/gettextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader method

Obtiene el texto del encabezado del campo del área de valores en la tabla dinámica.

```csharp
public override string GetTextOfDataFieldHeader()
```

### Valor de retorno

El texto del nombre del encabezado del campo de datos

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfDataFieldHeaderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de muestra para el contexto
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Crear una instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Obtener el texto predeterminado para el encabezado del campo de datos
                string dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Default data field header text: {dataFieldHeaderText}");

                // Establecer un texto personalizado para el encabezado del campo de datos
                settings.SetTextOfDataFieldHeader("Custom Data Header");
                dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Updated data field header text: {dataFieldHeaderText}");

                // Guarda el libro de trabajo
                workbook.Save("GetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("GetTextOfDataFieldHeader method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


