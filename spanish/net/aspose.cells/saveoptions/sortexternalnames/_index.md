---
title: "SaveOptions.SortExternalNames"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Indica si se ordenan los nombres definidos externamente antes de guardar el archivo"
type: docs
url: /es/net/aspose.cells/saveoptions/sortexternalnames/
---
## SaveOptions.SortExternalNames property

Indica si se ordenan los nombres definidos externos antes de guardar el archivo.

```csharp
public bool SortExternalNames { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SaveOptionsPropertySortExternalNamesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crear una instancia de OoxmlSaveOptions que hereda de SaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Mostrar el valor predeterminado de la propiedad SortExternalNames
                Console.WriteLine("Default SortExternalNames value: " + saveOptions.SortExternalNames);

                // Establecer SortExternalNames a true
                saveOptions.SortExternalNames = true;
                Console.WriteLine("SortExternalNames set to: " + saveOptions.SortExternalNames);

                // Guarde el libro de trabajo con las opciones de guardado especificadas
                workbook.Save("SortExternalNamesDemo.xlsx", saveOptions);

                Console.WriteLine("Workbook saved with SortExternalNames enabled.");
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

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


