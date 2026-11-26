---
title: "CustomProperty.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomProperty. Devuelve o establece el nombre del objeto"
type: docs
url: /es/net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Devuelve o establece el nombre del objeto.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar una propiedad personalizada con un nombre y un valor
                worksheet.CustomProperties.Add("SampleName", "SampleValue");

                // Recuperar la propiedad personalizada
                CustomProperty customProperty = worksheet.CustomProperties["SampleName"];

                // Mostrar el valor actual de la propiedad Name (operación de lectura)
                Console.WriteLine("Custom Property Name: " + customProperty.Name);

                // Establecer un nuevo valor para la propiedad Name
                customProperty.Name = "UpdatedName";
                Console.WriteLine("Updated Custom Property Name: " + customProperty.Name);

                // Guarda el libro de trabajo
                workbook.Save("NameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


