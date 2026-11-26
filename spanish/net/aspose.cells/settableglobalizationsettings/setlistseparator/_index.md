---
title: "SettableGlobalizationSettings.SetListSeparator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el separador para los parámetros de lista de la función ...etc"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setlistseparator/
---
## SettableGlobalizationSettings.SetListSeparator method

Establece el separador para la lista, los parámetros de la función, ...etc.

```csharp
public void SetListSeparator(char c)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| c | Carácter | el separador especificado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Llame al método SetListSeparator con un parámetro de carácter
                settings.SetListSeparator(';');
                
                // Aplicar la configuración al workbook
                workbook.Settings.GlobalizationSettings = settings;
                
                // Demuestre el efecto creando una fórmula con separador de lista
                worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
                worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
                
                Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
                Console.WriteLine("Formula using custom list separator created in cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("SetListSeparatorWithCharDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


