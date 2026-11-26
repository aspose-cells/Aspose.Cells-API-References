---
title: "SettablePivotGlobalizationSettings.SetTextOfEmptyData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Establece el texto de la etiqueta en blanco en la PivotTable"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextofemptydata/
---
## SettablePivotGlobalizationSettings.SetTextOfEmptyData method

Establece el texto de la etiqueta "(blank)" en la tabla dinámica.

```csharp
public void SetTextOfEmptyData(string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto de datos vacíos |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfEmptyDataWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos de ejemplo (opcional, solo para contexto)
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
                // Establezca texto personalizado para celdas de datos vacíos en una PivotTable
                settings.SetTextOfEmptyData("(no data)");

                // Verificar el cambio
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Custom text for empty data: {emptyDataText}");

                // (Opcional) Guarde el libro de trabajo – aunque no creamos una PivotTable,
                // Esto muestra que el libro de trabajo aún puede guardarse después de la manipulación de la configuración.
                workbook.Save("SetTextOfEmptyDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


