---
title: "WorkbookSettings.MaxUniqueItemsPerField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene y establece la limitación de elementos únicos por campo"
type: docs
url: /es/net/aspose.cells/workbooksettings/maxuniqueitemsperfield/
---
## WorkbookSettings.MaxUniqueItemsPerField property

Obtiene y establece la limitación de elementos únicos por campo

```csharp
public int MaxUniqueItemsPerField { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertyMaxUniqueItemsPerFieldDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            try
            {
                // Mostrar el valor actual de MaxUniqueItemsPerField
                Console.WriteLine("Current MaxUniqueItemsPerField value: " + settings.MaxUniqueItemsPerField);

                // Demostrar la configuración de un nuevo valor para MaxUniqueItemsPerField
                settings.MaxUniqueItemsPerField = 1000;
                Console.WriteLine("After setting to 1000: " + settings.MaxUniqueItemsPerField);

                // Establecer otro valor para mostrar que es mutable
                settings.MaxUniqueItemsPerField = 5000;
                Console.WriteLine("After setting to 5000: " + settings.MaxUniqueItemsPerField);

                // Agregar algunos datos de ejemplo para que el ejemplo tenga sentido
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Orange");

                // Guarda el libro de trabajo
                workbook.Save("MaxUniqueItemsPerFieldDemo.xlsx");
                Console.WriteLine("Workbook saved with MaxUniqueItemsPerField settings.");
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

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


