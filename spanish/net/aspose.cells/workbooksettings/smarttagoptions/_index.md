---
title: "WorkbookSettings.SmartTagOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene las opciones de la etiqueta inteligente"
type: docs
url: /es/net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

Obtiene las opciones de la etiqueta inteligente.

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();

                // Acceder a la configuración del libro de trabajo
                WorkbookSettings settings = workbook.Settings;

                // Lea la propiedad SmartTagOptions
                var smartTagOptions = settings.SmartTagOptions;

                // Muestre información sobre la instancia de SmartTagOptions
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // Opcionalmente, puede inspeccionar el estado predeterminado mediante ToString()
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // Guarde el libro de trabajo (el archivo contendrá la configuración predeterminada)
                workbook.Save("SmartTagOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


