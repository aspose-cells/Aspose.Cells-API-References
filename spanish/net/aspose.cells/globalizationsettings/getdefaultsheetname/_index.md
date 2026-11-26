---
title: "GlobalizationSettings.GetDefaultSheetName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de hoja predeterminado para agregar la hoja de cálculo automáticamente. El predeterminado es Sheet"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

Obtiene el nombre de hoja predeterminado para agregar la hoja de cálculo automáticamente. El valor predeterminado es "Sheet".

```csharp
public virtual string GetDefaultSheetName()
```

### Valor de retorno

el nombre de hoja predeterminado para agregar la hoja de cálculo automáticamente

### Observaciones

El nombre de la hoja agregada automáticamente (por ejemplo mediante [`Add`](../../worksheetcollection/add/)) será el nombre especificado más un número de secuencia. Por ejemplo, para un usuario de Alemania quizá quiera que el nombre de la hoja sea "Tabellenblatt2" en lugar de "Sheet2". Entonces el usuario puede implementar este método para devolver "Tabellenblatt".

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer configuraciones de globalización personalizadas
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Obtener el nombre de hoja predeterminado de la configuración personalizada de globalización
                string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
                Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");

                // Añadir una nueva hoja de cálculo para demostrar la nomenclatura basada en el valor predeterminado personalizado
                int sheetIndex = workbook.Worksheets.Add();
                Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
                Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");

                Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
        }
    }

    // Implementación de configuración personalizada de globalización
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDefaultSheetName()
        {
            return "CustomSheet"; // Custom default sheet name
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


