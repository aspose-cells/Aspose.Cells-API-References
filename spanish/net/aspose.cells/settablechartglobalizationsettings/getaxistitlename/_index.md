---
title: "SettableChartGlobalizationSettings.GetAxisTitleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Obtiene el nombre del Título para el Eje"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/getaxistitlename/
---
## SettableChartGlobalizationSettings.GetAxisTitleName method

Obtiene el nombre del título para el eje

```csharp
public override string GetAxisTitleName()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos mínimos para contexto
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            try
            {
                // Crea una instancia de SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Establecer un nombre de título de eje personalizado
                settings.SetAxisTitleName("Custom Axis Title");

                // Obtener el nombre del título del eje usando GetAxisTitleName
                string axisTitleName = settings.GetAxisTitleName();
                Console.WriteLine("Axis Title Name: " + axisTitleName);

                // Guarda el libro de trabajo
                workbook.Save("GetAxisTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetAxisTitleName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


